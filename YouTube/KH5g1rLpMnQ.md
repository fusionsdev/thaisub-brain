---
videoId: "KH5g1rLpMnQ"
title: "How to remove watermarks from Claude files"
channel: "Ray Fu"
url: "https://www.youtube.com/watch?v=KH5g1rLpMnQ"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-02"
tags: [thai-sub, youtube]
---

# How to remove watermarks from Claude files

> [!info] แหล่งที่มา
> Ray Fu · https://www.youtube.com/watch?v=KH5g1rLpMnQ

## 📝 สรุป

# สรุป: How to remove watermarks from Claude files
- **ช่อง:** Ray Fu · **ความยาว:** ~0.9 นาที · **ลิงก์:** https://www.youtube.com/watch?v=KH5g1rLpMnQ

## ประเด็นหลัก
- Claude Fable 5.1 ฝังลายน้ำ (watermark) ในทุกข้อความที่เขียน
- กลไก: ปกติโมเดลเลือกคำจากคะแนนความน่าจะเป็นที่เท่ากัน (สุ่ม) — ลายน้ำเปลี่ยนน้ำหนักให้คำบางคำถูกเลือกบ่อยกว่าโดยผู้อ่านมองไม่เห็น
- ในข้อความยาวๆ การเลือกคำนี้ก่อรูปแบบทางสถิติที่ตรวจจับได้
- API ตรวจจับเปิดให้เฉพาะหน่วยงานกำกับดูแล นักวิจัย และผู้บังคับใช้กฎหมาย — ไม่สาธารณะ
- จุดอ่อน: ตรวจโค้ดได้ไม่ดี แต่แรงกับย่อหน้า/บทความยาว
- การแก้เล็กน้อยไม่พอ เพราะรูปแบบกระจายทั้งเรื่อง — ต้อง rewrite ทั้งหมด
- ใช้ GPT/Gemini rewrite ก็ไม่พอ เพราะโมเดลใหญ่ทุกตัวมีลายน้ำเช่นกัน
- วิธีที่เสนอ: รัน local model (เช่น Llama) บนเครื่องตัวเอง ให้ Claude เขียนแล้วส่งให้โมเดลท้องถิ่น rewrite — ได้ข้อความไม่มีลายน้ำ ทำอัตโนมัติได้
- รับคู่มือติดตั้งโมเดลท้องถิ่นฟรีโดยกดไลก์ + คอมเมนต์ "mark"

## ความเห็นสรุป
อธิบายหลักการ watermark ทางสถิติได้เข้าใจง่าย และวิธีเอาออกด้วยโมเดลท้องถิ่นก็มีลอจิกที่ฟังขึ้น แต่ควรระวังว่าการลบลายน้ำอาจขัดกับข้อกำหนดการใช้บริการของผู้ให้บริการโมเดลครับ

เสียงพากย์ไทย: ![[KH5g1rLpMnQ.mp3]]

