---
videoId: "SSj2J9kfKn8"
title: "How to Self-Host a Community Relay in Buzz (Complete Local Setup)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=SSj2J9kfKn8"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# How to Self-Host a Community Relay in Buzz (Complete Local Setup)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=SSj2J9kfKn8

## 📝 สรุป

# สรุป: How to Self-Host a Community Relay in Buzz (Complete Local Setup)

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~15 นาที · **ลิงก์:** https://www.youtube.com/watch?v=SSj2J9kfKn8

## ประเด็นหลัก

- **โฮสต์เอง vs. ให้ Block โฮสต์:** ความแตกต่างใหญ่คือ "ใครเป็นเจ้าของเครื่องที่ให้บริการ" — keys และ events ยังเป็นของคุณทั้งสองแบบ แต่ custody (ดิสก์/backup/การควบคุม) เปลี่ยนไป
- **Community relay คืออะไร:** ใน Buzz, relay ก็คือ community — เป็นเซิร์ฟเวอร์ที่เก็บ signed events, media, และ Git repos
- **ข้อดีของ self-hosting:** ควบคุมได้ทุกอย่าง — ตั้งค่า relay-level policy, closed owner mode, moderation dashboard, ข้อมูลทั้งหมดเป็นไฟล์บนดิสก์คุณเอง
- **ข้อเสียของ self-hosting:** ต้องดูแล backup เอง, pin เวอร์ชัน, จัดการ TLS และ uptime — มี maintenance เพิ่ม
- **รูปแบบการ deploy:** VPS (ออนไลน์ 24/7), PC โลคอล (เฉพาะคุณกับเอเจนต์โลคอล), home box + Tailscale VPN (เฉพาะอุปกรณ์ใน tailnet), Railway (คลิกเดียว แต่ใช้ฮาร์ดแวร์เขา)
- **ขั้นตอนตั้งค่าแบบโลคอล:** ต้องมี Docker Desktop, Docker Compose, WSL → clone GitHub repo ของ Buzz → แก้ไขไฟล์ ENV (ตั้ง secrets, pub key, พอร์ต) → รัน `docker compose up` จาก Git Bash
- **ทดสอบการทำงาน:** Buzz เชื่อมต่อกับ relay โลคอล → เพิ่มเอเจนต์ → สร้าง channel → ส่งข้อความ/สร้างโปรเจกต์ → ทำงานได้แม้ปิด Wi-Fi
- **เครื่องมือตรวจสอบ:** Adminer (ดูฐานข้อมูล Postgres), MinIO console (ดู media storage), Docker logs (ดู signed events)
- **ทีเด็ด:** self-hosting skill บน Buzz skills repo — รวม issues และ pitfalls ที่เจอระหว่างทำ

## ความเห็นสรุป

วิดีโอนี้สอนวิธี self-host Buzz community relay ได้อย่างครบถ้วนและปฏิบัติได้จริง — ตั้งแต่แนวคิดไปจนถึงมือทำ ผู้พูดอธิบายข้อดีข้อเสียอย่างตรงไปตรงมา พร้อมสาธิตการทำงานแบบออฟไลน์ให้เห็นผลชัดเจน เหมาะสำหรับคนที่อยากควบคุมข้อมูลของตัวเองเต็มที่ แต่ต้องยอมรับภาระ maintenance เพิ่มขึ้นมาบ้าง

เสียงพากย์ไทย: ![[SSj2J9kfKn8.mp3]]

