---
videoId: "VsJDLvdGGqM"
title: "Jack Dorsey's BUZZ:  The Open Source Slack + Hermes Agent + Claude Code"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=VsJDLvdGGqM"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Jack Dorsey's BUZZ:  The Open Source Slack + Hermes Agent + Claude Code

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=VsJDLvdGGqM

## 📝 สรุป

# สรุป: Jack Dorsey's BUZZ:  The Open Source Slack + Hermes Agent + Claude Code

ช่อง: DevsKingdom · ความยาว: 23 นาที 44 วินาที · ลิงก์: https://www.youtube.com/watch?v=VsJDLvdGGqM

- วิดีโอนี้เป็นบทช่วยสอนแนะนำโปรเจกต์ Buzz แพลตฟอร์ม Slack แบบโอเพนซอร์สที่สร้างโดยทีม Block (บริษัทของ Jack Dorsey) ภายใต้สัญญาอนุญาต Apache 2.0 ซึ่งได้รับความนิยมอย่างรวดเร็ว
- ผู้พูดสาธิตการใช้งาน Buzz ผ่าน Buzz CLI และการเชื่อมต่อ AI agent (Claude) เข้ากับแพลตฟอร์มผ่าน ACP โดยมี Buzz relay เป็นเกตเวย์กลางที่เชื่อม Postgres, Redis และ storage แบบ S3 (MinIO)
- อธิบายการตั้งค่า relay แบบง่าย ๆ: ตั้ง environment variables และ private key ของ Buzz relay แล้วใช้งานบนพอร์ต 3000 ได้ทันที พร้อมการสร้าง channel และส่งข้อความผ่านคำสั่ง buzz CLI
- สาธิตการสร้าง workflow แบบมีเงื่อนไข (conditional workflow) ในรูปแบบไฟล์ YAML เช่น ถ้าข้อความมีแท็ก P1 หรือ SEV1 จะ trigger การส่งข้อความไปที่ channel "P1 escalation" แต่ถ้าไม่มีจะไปที่ "normal path"
- อธิบายแนวคิดการยืนยันตัวตนของ Buzz ด้วยคู่ public key กับ secret key และการสร้าง user ใหม่ (เช่น Alice/Alex) พร้อมการเพิ่ม member เข้า channel
- สาธิตการผูก AI agent กับ user ผ่าน ACP (เช่น Claude agent ACP) ทำให้ agent ตอบกลับข้อความใน channel โดยอัตโนมัติ เช่น การถาม "How are you?" แล้ว agent ตอบกลับพร้อมแนะนำความสามารถของตัวเอง
- ผู้พูดย้ำว่าทุกอย่างสามารถทำงานอัตโนมัติได้เต็มรูปแบบ ทั้ง agentic workflows, agentic pipelines และ agentic communities บนแพลตฟอร์มโอเพนซอร์ส
- ปิดท้ายด้วยการติดตั้งแบบไม่ใช้ Docker ทีละขั้นตอน: ติดตั้ง Postgres, Redis, Rust, MinIO (พร้อม systemd service และ bucket) จากนั้น clone repo และรัน cargo build เพื่อ build relay CLI, Buzz admin และ Buzz ACP
- ขั้นตอนสุดท้ายคือการตั้งค่า environment ของ Buzz relay (bind address, database URLs, S3 storage, คู่ private/public key) แล้วรัน buzz relay พร้อมทดสอบผ่าน health endpoint และพอร์ต 9090 (readiness/liveness)

**ความเห็น:** วิดีโอเป็นบทช่วยสอนที่กระชับและใช้งานได้จริง เหมาะสำหรับคนที่อยาก self-host แพลตฟอร์มแชตแบบ Slack ที่เชื่อมต่อกับ AI agent ได้เอง โดยเฉพาะการติดตั้งแบบไม่มี Docker ที่หาเอกสารอธิบายที่อื่นไม่ได้ ข้อควรระวังคือชื่อวิดีโอเอ่ยถึง Hermes Agent และ Claude Code แต่ในเนื้อหาจริง ๆ กล่าวถึงเฉพาะการเชื่อมต่อ Claude ผ่าน ACP เท่านั้น

เสียงพากย์ไทย: ![[VsJDLvdGGqM.mp3]]

