---
videoId: "lbDgO78Z5go"
title: "Feeding GBrain Your Emails Autonomously with Hermes Agent"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=lbDgO78Z5go"
published: "2026-07-14"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Feeding GBrain Your Emails Autonomously with Hermes Agent

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=lbDgO78Z5go

## 📝 สรุป

# สรุป: Feeding GBrain Your Emails Autonomously with Hermes Agent
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~17 นาที · **ลิงก์:** https://www.youtube.com/watch?v=lbDgO78Z5go

## ประเด็นหลัก
- วิดีโอนี้สอนวิธีเชื่อมต่ออีเมล Gmail เข้ากับ GBrain โดยอัตโนมัติผ่าน Hermes Agent โดยใช้ Google Workspace CLI (GWS) ซึ่งเป็น Rust binary ตัวเดียวที่จัดการ Gmail, Calendar, Drive, Docs ได้ครบ
- หลักการสำคัญ: "สคริปต์เก็บข้อมูล, agent ตัดสินใจ, สมองกลจดจำ" — สคริปต์ทำหน้าที่เก็บอีเมลเท่านั้น ส่วนการเขียนเข้า GBrain ทั้งหมดผ่าน MCP ในรอบการทำงานของ agent
- การตั้งค่าเริ่มต้น: ติดตั้ง gcloud CLI และ GWS ใน WSL, ล็อกอิน, สร้าง OAuth client แบบ desktop app, อนุญาตสิทธิ์ดูอีเมลเท่านั้น
- collector script (check_inbox.py) ดึงอีเมลของวันนี้, กรองขยะ, จำ message ID, สร้าง Gmail deep link เองในโค้ด — ไม่เรียก LLM ไม่เดา URL
- รูปแบบการเขียนหน้า GBrain สำคัญมาก: ต้องมี typed front matter, wiki link ของผู้ส่ง, คำพูดสำคัญที่ยกมาตรงตัว, deep link ไปยังอีเมลต้นฉบับ — ไม่ใช่ก้อนข้อความสรุปทั่วไป
- การตั้งค่า Hermes cron job แบบ daily โดยใช้ check_inbox.py เป็น pre-run script และใช้ Grok 4.5 เป็น agent
- มาตรการรักษาความปลอดภัย 3 ชั้น: collector gate (allow list เท่านั้น), protocol gate (อัปเดตเฉพาะหน้าที่มีอยู่ ห้ามสร้าง entity ใหม่), และการส่ง digest ไป Telegram เพื่อตรวจทัน
- ผลลัพธ์: สามารถถาม Hermes เรื่องที่ไม่เคยคุยกันโดยตรงได้ เพราะมันมีข้อมูลจากอีเมล/newsletter แล้ว
- วิดีโอหน้าจะพูดถึงการใช้ Fathom transcript กับ GBrain

## ความเห็นสรุป
วิดีโอนี้เป็นคู่มือปฏิบัติที่ค่อนข้างละเอียดสำหรับการเชื่อมต่ออีเมลเข้า GBrain ผ่าน Hermes Agent ครับ จุดเด่นคือการเน้นย้ำถึงความสำคัญของรูปแมบบข้อมูลที่ถูกต้อง และมาตรการรักษาความปลอดภัยที่ออกแบบมาเพื่อป้องกันข้อมูลขยะหรือ prompt injection แม้ว่าการตั้งค่าเริ่มต้นจะมีหลายขั้นตอน แต่เมื่อตั้งค่าเสร็จแล้วระบบจะทำงานอัตโนมัติได้จริง ทำให้ GBrain มีข้อมูลที่หลากหลายและครอบคลุมมากขึ้น

เสียงพากย์ไทย: ![[lbDgO78Z5go.mp3]]
