---
videoId: "kP47nEyISf0"
title: "Testing Drama 3: Can a Local TTS Model Create the Perfect Voice Clone?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=kP47nEyISf0"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-10-22"
tags: [thai-sub, youtube]
---

# Testing Drama 3: Can a Local TTS Model Create the Perfect Voice Clone?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=kP47nEyISf0

## 📝 สรุป

# สรุป — Testing Drama 3: Can a Local TTS Model Create the Perfect Voice Clone?

- ทดสอบ Drama 3 จาก Fish Audio — โมเดล TTS แบบ open weights ขนาด 35B params (active 3B/token) ใช้พื้นที่ ~70 GB บน DGX Spark แบบ full size
- ทดสอบ inline sound tags ควบคุมอารมณ์เสียง (sigh, pause, loud laugh, emphasis, fast) — ส่วนใหญ่ทำงานได้ดี เสียงฟังดูเป็นธรรมชาติกว่า TTS รุ่นก่อน ๆ
- ทดสอบการสลับภาษา — ใช้แท็กภาษาญี่ปุ่นกับข้อความญี่ปุ่นจริงได้สำเร็จ โดยไม่เปลี่ยน character ของเสียง
- Voice cloning — ลองโคลนเสียงตัวเองจากคลิปอ้างอิงหลายชุด ได้ผลใกล้เคียงระดับหนึ่ง (clone C ใกล้สุด) แต่ยังมีจุดที่ฟังออกว่าไม่ใช่เสียงจริง
- ปรับแต่งเพิ่มด้วย pitch shift (ผิดเพี้ยน) และ direction tag "slightly deeper" (ได้ผลดีกว่า)
- ผลลัพธ์สุดท้าย: voice clone ที่ใช้ direction tags + inline sound tags ทำได้ใกล้เคียงเสียงจริงมาก เสียงเป็นธรรมชาติ ไม่ใช่หุ่นยนต์
- ใช้เวลา generate ~15 วินาที สำหรับคลิป 14-15 วินาที — เร็วมากเมื่อรัน locally

** verdict: ** Drama 3 เป็นโมเดล TTS ที่น่าประทับใจสำหรับรันบนเครื่องตัวเอง — voice cloning ใกล้เคียงใช้ได้, inline emotion tags ทำงานได้จริง, และ inference เร็วมาก จุดอ่อนคือ clone ยังไม่สมบูรณ์แบบ 100% และบางฟีเจอร์ต้องใช้ผ่านเว็บไซต์แทน local

