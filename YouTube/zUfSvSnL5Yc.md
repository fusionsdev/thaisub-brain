---
videoId: "zUfSvSnL5Yc"
title: "OmniRoute: The Ultimate Unified Open Source AI Gateway"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=zUfSvSnL5Yc"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# OmniRoute: The Ultimate Unified Open Source AI Gateway

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=zUfSvSnL5Yc

## 📝 สรุป

# สรุป: OmniRoute: The Ultimate Unified Open Source AI Gateway

- ช่อง: DevsKingdom · ความยาว: 10:15 นาที · ลิงก์: https://www.youtube.com/watch?v=zUfSvSnL5Yc
- OmniRoute คือ AI gateway แบบโอเพนซอร์สที่รวมผู้ให้บริการ AI ทั้งหมดไว้ในแพลตฟอร์มเดียว ใช้ endpoint เดียวกันเข้าถึงผู้ให้บริการทุกราย ทั้งแบบฟรีและเสียเงิน
- โปรเจกต์มีดาว (stars) บน GitHub ราว 33,000 ดาว และอ้างว่าเป็น "free AI gateway" พร้อมระบบจัดเส้นทางอัตโนมัติด้วย 19 กลยุทธ์ และเป็น repository อันดับ 1 ของวัน
- วิดีโอสอนติดตั้ง OmniRoute ทีละขั้นตอนบน Kaggle แบบฟรี 100% โดยไม่ต้องใช้ GPU หรือซื้อ virtual private machine
- ขั้นตอนแรก: ติดตั้ง NPM สำหรับ Node.js (ต้องเป็นเวอร์ชันใหม่กว่า 24 ขึ้นไป เช่น 25) จากนั้นติดตั้งและเริ่มรัน Nginx
- ตั้งค่า Nginx ให้ route ทราฟฟิกไปที่พอร์ต 2128 และพอร์ตสตรีมมิง (live socket port) ไปที่พอร์ต 2132
- บน Kaggle ต้องติดตั้ง local terminal เพื่อเปิดลิงก์สาธารณะ แล้วคัดลอก public URL ไปใส่ใน environment ของ OmniRoute ทั้ง next public base URL และ next public live web socket URL (ใช้ WSS)
- เมื่อรันบน production ต้องเปลี่ยน initial password ก่อนล็อกอินเข้าสู่แพลตฟอร์ม
- รัน npm run build เพื่อสร้าง production build (Kaggle ให้แรมฟรี 30 กิกะไบต์) แล้วเช็คว่า build ID พร้อม จากนั้นรัน npm run start เพื่อเปิดใช้งาน
- เพิ่มผู้ให้บริการได้ที่ส่วน provider เช่น Llama, Grok, Kimiko, Amazon, Claude Code client, Tech Gravity, Minimax, GLN รวมราว 296 ผู้ให้บริการ
- ทดสอบได้โดยระบุ model เป็น auto ระบบจะเลือกโมเดลให้อัตโนมัติ เช่น felo chat หรือ north mini code free หรือระบุโมเดลเจาะจงอย่าง Minimax M3 โดยต้องตั้งค่า prefix สำหรับโมเดลแบบกำหนดเอง
- verdict: วิดีโอแนะนำโปรเจกต์ที่ใช้งานได้จริงและติดตั้งง่าย เหมาะกับคนที่อยากลองใช้ AI gateway รวมศูนย์ฟรีบน Kaggle โดยไม่ต้องเสียเงิน

เสียงพากย์ไทย: ![[zUfSvSnL5Yc.mp3]]

