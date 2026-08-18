---
videoId: "nz-p2JS9RJc"
title: "OpenWork's Cloud Collaboration System"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=nz-p2JS9RJc"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# OpenWork's Cloud Collaboration System

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=nz-p2JS9RJc

## 📝 สรุป

# สรุป: OpenWork's Cloud Collaboration System

ช่อง: DevsKingdom · ความยาว: 13 นาที · ลิงก์: https://www.youtube.com/watch?v=nz-p2JS9RJc

- วิดีโอแนะนำ OpenWork Dam ซึ่งเป็นคอนโทรลเพลน (control plane) สำหรับจัดการ OpenWork (ทางเลือกโอเพนซอร์สแทน Clockwork) ครอบคลุมทั้งทีมและองค์กร
- ฟีเจอร์หลัก: จัดการสมาชิกและทีม, จัดการสิทธิ์การเข้าถึงจากที่เดียว, ตั้งค่านโยบายไฟล์, จำกัดการเข้าถึงโมเดลในเครื่อง, เผยแพร่สกิลและปลั๊กอินผ่าน marketplace
- ตอนนี้ OpenWork Dam รองรับเฉพาะแอปพลิเคชันเดสก์ท็อป (ดาวน์โหลด OpenWork Enterprise ผ่านหน้า Open Store) ยังไม่รองรับเว็บแอปพลิเคชัน
- เชื่อมต่อผู้ให้บริการโมเดลได้หลายเจ้า (OpenAI, Anthropic, Pooder และอื่นๆ) ผ่านปุ่ม add provider พร้อมเลือกได้ว่า admins เพิ่มผู้ให้บริการเองได้ไหม
- เพิ่ม/ลบสมาชิกด้วยการกรอกอีเมลเพื่อเชิญเข้าร่วมทีม และติดตามเมตริกในหน้า analytics เช่น ผู้ใช้ที่ใช้งานอยู่, เซสชันต่อสัปดาห์, งานต่อสัปดาห์
- หน้า settings มี API keys, SSO, desktop policies, diagnostics และข้อมูลทั่วไป
- การติดตั้งฝั่งเซิร์ฟเวอร์: ติดตั้ง MySQL server + Node, ตั้งค่าฐานข้อมูล, clone repository แล้วรัน npm install และ build แพ็กเกจ (email, MCP client, DenDB, Den API)
- ตั้งค่า environment อย่างละเอียด: database URL, คีย์ยืนยันตัวตน, API public URL, CORS, โหมดองค์กร (single/multi), และ seed URL สำหรับผู้ใช้ทดสอบ
- migrate ฐานข้อมูลด้วยคำสั่งบรรทัดเดียว (DB migrate ธรรมดาใช้ไม่ได้) แล้วตรวจสอบตารางด้วย show tables
- สำหรับโปรดักชัน: สร้าง systemd หรือ supervisor, รันด้วยโปรดักชันบิลด์, ใช้ Nginx reverse proxy และรันเว็บด้วย NX start (build ด้วย Next.js)
- กระบวนการ seed ผู้ใช้ทดสอบ (เช่น Alice ที่ acme.test) ต้องสลับ app mode ระหว่างโปรดักชัน (0) กับโหมดพัฒนา (1) และเปิด allow public sign up ก่อน
- ปิดท้ายด้วยวิธีติดตั้งแอปเดสก์ท็อปบนเครื่องโลคอลแล้วเชื่อมต่อกับคอนโทรลเพลนกลาง

**ความเห็น:** วิดีโอสาธิตที่ละเอียดและทำตามได้จริงสำหรับคนที่ต้องการติดตั้งและรัน OpenWork Dam ด้วยตัวเอง แต่ไม่เกี่ยวข้องกับผู้ใช้เว็บแอปพลิเคชัน และชื่อแบรนด์/ศัพท์เทคนิคบางตัวมาจากคำบรรยายอัตโนมัติ อาจคลาดเคลื่อนจากชื่อจริงได้

เสียงพากย์ไทย: ![[nz-p2JS9RJc.mp3]]

