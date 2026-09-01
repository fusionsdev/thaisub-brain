---
videoId: "OHaYGPiZQ3g"
title: "First Look at GPT-5.6: The Ultimate Hermes Agent Driver?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=OHaYGPiZQ3g"
published: "2026-07-09"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# First Look at GPT-5.6: The Ultimate Hermes Agent Driver?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=OHaYGPiZQ3g

## 📝 สรุป

# สรุป: First Look at GPT-5.6: The Ultimate Hermes Agent Driver?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~17 นาที · **ลิงก์:** https://www.youtube.com/watch?v=OHaYGPiZQ3g

## ประเด็นหลัก

- OpenAI เปิดตัว GPT-5.6 อย่างเป็นทางการ โดยมีโมเดลย่อยสามตัว: Sol (flagship), Terra (สมดุลสำหรับงานประจำวัน), Luna (ประหยัดต้นทุน)
- มีโหมดเสริม compute สองแบบ: max (ให้โมเดลเดียว reason นานขึ้น) และ ultra (แบ่งงานออกเป็น agent ขนาน — research, implementation, testing, critique)
- ในเบนช์มาร์ก Agents' Last Exam ได้ 53.6 คะแนน สูงกว่า Fable ถึง 13.1 คะแนนบน AI Intelligence Index ขณะที่เร็วกว่า 61% และต้นทุนครึ่งหนึ่ง
- คุณสมบัติเด่นคือ programmatic tool calling — เขียนและรันโปรแกรมใน memory เพื่อประสาน tool ทำให้ลด model round-trip และ prompt token
- ด้าน coding นำใน agentic coding และงาน terminal แบบกว้าง แต่ Fable ยังเหนือกว่าใน SWE-bench แบบหลายไฟล์ยาก ๆ
- ด้านความปลอดภัยไซเบอร์กระโดดขึ้นมาก (ExploitBench จาก 47.9% เป็น 73.5%) แต่มี guardrail ที่เข้มงวดกว่า
- ราคา Sol: $5 input / $30 output; Terra & Luna: $1 input / $6 output (ใกล้เคียง Haiku)
- ทดสอบ one-shot สร้างเกม One Piece x Star Wars ใน Hermes Agent: ผลออกมาดีมาก สไตล์ต่างจากโมเดลอื่น มีรายละเอียดมาก อยู่ในระดับเทียบเท่าหรือดีกว่า Fable แม้ headline stagger จะยังไม่สมบูรณ์
- ทดสอบ audit codebase โปรเจกต์ Shovels Terminal ด้วย ultra ใน Codex: พบ bug high severity 4 ตัว
- นำ bug ที่พบไปให้ Fable verify — ผลคือทั้ง 14 รายการเป็นจริงตามข้อเท็จจริง และ 12 รายการเป็นการพบที่ถูกต้อง
- บาง bug เป็นโค้ดที่ Fable เขียนเองแล้วไม่รู้ตัวว่ามี bug — แสดงให้เห็นคุณค่าของการมี auditor คนที่สอง
- context window ใน Hermes Agent เพิ่มจาก 270K เป็น 372K token ช่วยในงาน coding ระยะยาว

## ความเห็นสรุป

GPT-5.6 ผลิตงาน front-end ได้น่าประทับใจมากในการลองครั้งแรก และในฐานะ code auditor มันสามารถจับ bug ที่แม้แต่โมเดลระดับสูงอย่าง Fable ก็พลาดได้ ผู้จัดจะใช้มันเป็น driver หลักใน Hermes Agent ต่อไป และเน้นย้ำว่าการมี auditor สองชั้นจำเป็นมากเพราะแม้โมเดลเก่งสุดก็ยังเขียน bug โดยไม่รู้ตัว ทั้งหมดนี้เป็นแค่การลองครั้งแรก ผลลัพธ์จะต้องติดตามกันต่อไปในการใช้งานจริง

เสียงพากย์ไทย: ![[OHaYGPiZQ3g.mp3]]
