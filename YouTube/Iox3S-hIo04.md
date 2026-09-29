---
videoId: "Iox3S-hIo04"
title: "Day 4B: Agent Project Build — Complete Multi-Agent Demo (Start to Finish)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=Iox3S-hIo04"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 4B: Agent Project Build — Complete Multi-Agent Demo (Start to Finish)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=Iox3S-hIo04

## 📝 สรุป

# สรุป: Day 4B: Agent Project Build — Complete Multi-Agent Demo (Start to Finish)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~20 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Iox3S-hIo04

## ประเด็นหลัก

- แม้ชื่อวิดีโอจะระบุ Agent Project Build แต่เนื้อหาจริงคือ agent evaluation (การประเมินผลเอเจนต์) — ส่วน B ของ assignment Day 4
- Observability เป็นแบบ reactive (ทำงานหลังปัญหาเกิด) ส่วน evaluation คือการประเมินประสิทธิภาพอย่างต่อเนื่องเพื่อรับรู้ quality regression ได้ล่วงหน้า
- ความต่างจากการทดสอบซอฟต์แวร์เดิม: standard testing = ทดสอบ happy path ส่วน evaluation = ประเมินกระบวนการตัดสินใจทั้งเส้นทาง (trajectory) ของเอเจนต์
- กรณีศึกษา: home automation agent ที่ instructions ตั้งใจให้มั่นใจเกินจริง (อ้างว่าควบคุมอุปกรณ์ได้ทุกชนิด) — ผ่าน test พื้นฐานแต่ซ่อนข้อบกพร่อง
- การสร้าง evaluation ใน ADK web UI: ถามเอเจนต์ → บันทึก session เป็น eval case ใน eval set → กด run evaluation
- คะแนนสำคัญ 2 ตัว: response match score (ความคล้ายของคำตอบจริงกับคำตอบที่คาดหวัง 1.0 = ตรงสนิท) และ tool trajectory score (ความถูกต้องของ tool + parameter + ลำดับการเรียก 1.0 = สมบูรณ์แบบ)
- การทดสอบให้พังโดยเจตนา (แก้ expected response เป็น "โคมไฟปิดอยู่") แสดงผล fail สีแดง พร้อม tooltip เทียบ actual vs expected — feedback แบบนี้มีค่ามากสำหรับ debug
- การทดสอบทีละบทสนทนาใน UI scale ไม่ได้ — ต้องใช้ systematic evaluation ด้วยหลาย test case รวมเป็น evaluation set (ไฟล์ JSON)
- Regression testing = รัน test เดิมซ้ำเพื่อยืนยันว่าการเปลี่ยนแปลงใหม่ไม่ทำลายของเดิม; ADK รองรับ pytest และ ADK eval ผ่านคำสั่ง CLI
- ขั้นตอน evaluation 4 ขั้น: สร้าง evaluation configuration (นิยาม metric + เกณฑ์ผ่าน/ตก) → สร้าง test case → รันเอเจนต์ด้วย test query → เปรียบเทียบผลลัพธ์
- User simulation (optional): ใช้โมเดล genai อย่าง Gemini สร้าง prompt ของ user แบบไดนามิกระหว่าง evaluate ช่วยค้นพบ edge case ที่ static test case มักพลาด

## ความเห็นสรุป

วิดีโอนี้อธิบาย evaluation ได้เป็นขั้นเป็นตอนดี โดยเฉพาะการพาสร้าง test จริงใน web UI แล้วทำให้มัน fail ให้ดู ช่วยให้เข้าใจคะแนนทั้งสองแบบได้รวดเร็วครับ จุดที่ผู้เรียนควรเก็บกินคือแนวคิด systematic evaluation ด้วย JSON และ regression testing เพราะเป็นสะพานสู่งานจริงใน production ครับ ข้อควรระวังอีกครั้ง: ชื่อวิดีโอไม่ตรงกับเนื้อหาจริง (ชื่อบอก Project Build แต่สอน Evaluation) ควรใช้เนื้อหาในคลิปเป็นหลักครับ

เสียงพากย์ไทย: ![[Iox3S-hIo04.mp3]]

