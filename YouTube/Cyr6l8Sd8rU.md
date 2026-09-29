---
videoId: "Cyr6l8Sd8rU"
title: "Day 3A: Agent Memory Explained — Sessions, Long-Term Context & Recall"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=Cyr6l8Sd8rU"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 3A: Agent Memory Explained — Sessions, Long-Term Context & Recall

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=Cyr6l8Sd8rU

## 📝 สรุป

# สรุป: Day 3A: Agent Memory Explained — Sessions, Long-Term Context & Recall
- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~20 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Cyr6l8Sd8rU

## ประเด็นหลัก
- แบบฝึกหัด Day 3 Part A ของคอร์ส Google × Kaggle 5-Day AI Agents Intensive พาทำ stateful agent ด้วย session และ context engineering ใน ADK
- LLM ทุกตัว stateless โดยธรรมชาติ — รู้เฉพาะข้อมูลในการเรียก API ครั้งเดียว จึงต้องใช้ session เป็นความจำระยะสั้น และ memory เป็นความจำระยะยาว
- Session คือภาชนะบรรจุบทสนทนาของ user หนึ่งคนกับ agent หนึ่งตัว ประกอบด้วยสองส่วนคือ event (input, คำตอบ, tool call, ผลลัพธ์) และ state (scratchpad key-value ที่ tool ทุกตัวเข้าถึงได้)
- เปรียบเทียบให้เห็นภาพ: session คือสมุดบันทึก, event คือรายการในหน้า, session service คือตู้แฟ้ม, runner คือผู้ช่วยบริหารการสนทนา
- InMemorySessionService เก็บใน RAM จึงลืมทุกอย่างเมื่อรีสตาร์ท kernel — demo พิสูจน์ด้วยการรีสตาร์ทแล้ว agent ตอบว่าจำอดีตไม่ได้
- ทางเลือก session service สามแบบ: InMemory (dev/ทดสอบ), Database (self-managed, อยู่รอดการรีสตาร์ท), Agent Engine (production บน GCP แบบ fully managed)
- อัปเกรดเป็น DatabaseSessionService ด้วย SQLite (ไฟล์ในเครื่อง ไม่ต้องมี DB server) แล้วทดสอบว่า session แยกส่วนจริง — session 02 ไม่รู้จักชื่อที่บอกไว้ใน session 01
- Context compaction ใช้ EventCompactionConfig (interval และ overlap size) ให้ runner สรุปย่อประวัติเก่าโดยอัตโนมัติ — ไม่ลบ event เก่าแต่แทนที่ด้วย event เดียวที่บรรจุสรุป ช่วยลด cost และเพิ่มความเร็ว
- ตัวเลือกขั้นสูงเพิ่มเติม: custom sliding window compactor (ควบคุม summarization prompt หรือใช้ LLM เฉพาะทาง) และ gzip context (บีบอัด static instructions ให้เล็กลง)
- การจัดการ session state ด้วย custom tool: สร้าง save_user_info / retrieve_user_info เก็บ username กับ country ผ่าน tool context — ข้อมูลแนะนำครั้งเดียวแต่อ้างอิงได้ตลอดบทสนทนา
- Cross-session state sharing: สร้าง session ใหม่โดยยก state จาก session ก่อนหน้ามาใช้ได้ เช่น ชื่อ Sam และประเทศ Poland

## ความเห็นสรุป
วิดีโอนี้อธิบายแนวคิด session/state/compaction ได้เชื่อมโยงกันดีมาก จุดเด่นคือการพิสูจน์ความขี้ลืมของ in-memory agent ด้วยการรีสตาร์ท kernel จริง ๆ แล้วค่อยแก้ด้วย SQLite ทีละขั้น ทำให้เห็นปัญหาและทางแก้อย่างจับต้องได้ ส่วน context compaction กับ session state tool เป็นพื้นฐานสำคัญของ context engineering ที่จำเป็นต่อการทำ agent ใช้งานจริงใน production ครับ

เสียงพากย์ไทย: ![[Cyr6l8Sd8rU.mp3]]

