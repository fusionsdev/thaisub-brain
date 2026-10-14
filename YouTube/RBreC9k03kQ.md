---
videoId: "RBreC9k03kQ"
title: "How to Use Your Claude Sub in Hermes Agent"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=RBreC9k03kQ"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-10-15"
tags: [thai-sub, youtube]
---

# How to Use Your Claude Sub in Hermes Agent

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=RBreC9k03kQ

## 📝 สรุป

# สรุป: How to Use Your Claude Sub in Hermes Agent

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~11 นาที · **ลิงก์:** https://www.youtube.com/watch?v=RBreC9k03kQ

## ประเด็นหลัก

- Claude เคยถูกใช้เป็นโมเดลใน agent ผ่าน token แต่ Anthropic ยกเลิกการใช้งานรูปแบบนั้นไปแล้ว ทำให้ผู้ใช้ต้องหันไปใช้โมเดลอื่นแทน
- Nous Research ออกปลั๊กอิน Claude Subscription Direct SDK ที่ช่วยให้ใช้ Claude models ผ่าน Claude Code CLI ที่ล็อกอินอยู่ได้อย่างถูกต้องตาม Terms of Service
- วิธีติดตั้งมี 3 ทาง: (1) ผ่านแท็บ Capabilities > Plugins ใน Hermes Desktop แล้วกด Add to Agent (2) ผ่านคำสั่ง terminal `hermes plugins install claude-subscription-direct-sdk` (3) สั่งให้ Hermes ติดตั้งให้จากในแชทโดยตรง
- หลักการทำงาน: Claude เป็น "สมอง" (model backend) ส่วน Hermes เป็น "agent" ที่รับผิดชอบ tool execution, approvals, delegation, memory, skills และ session management ทั้งหมด — Claude เป็นแค่ transport ไม่ใช่ agent
- เมื่อเทียบกับ T3 Code และ Buzz: ในสองตัวนั้น Claude เป็น agent จริง ๆ (Claude runtime รัน tools) แต่ใน Hermes Direct SDK นั้น Claude เป็นแค่ transport ส่วน Hermes เป็นคนรัน agent loop
- ปลั๊กอินพูด native stream JSON โดยตรง ไม่ต้องใช้ Python Agent SDK package จาก Claude — ขับเคลื่อนเฉพาะ Claude Code executable ที่ไม่ได้แก้ไข
- การทดสอบ side-by-side ระหว่าง Claude Code โดยตรงกับ Hermes Agent (ทั้งคู่ใช้ Opus 5.5) พบว่า Hermes ให้คำตอบสุดท้ายเร็วกว่าและกระชับกว่า (อาจเพราะการตั้งค่า SOUL.md)
- ขณะนี้เป็น experimental — replay behavior ขึ้นกับเวอร์ชัน CLI และ Anthropic อาจเปลี่ยนนโยบายได้ในอนาคต

## ความเห็นสรุป

ปลั๊กอินนี้แก้ pain point ใหญ่ของผู้ใช้ Hermes Agent ที่ต้องการใช้ Claude models โดยไม่ต้องเสียเงินเพิ่มและไม่ผิด TOS วิธีติดตั้งทำได้ง่ายมากจากในแชทหรือ UI โดยตรง และเมื่อใช้แล้วประสิทธิภาพไม่ได้ด้อยไปกว่า Claude Code เลยแม้แต่น้อย — ในทางกลับกัน Hermes ยังเสริมความสามารถด้าน memory, skills และ agent loop ที่ Claude Code ไม่มี ถือเป็น win-win สำหรับคนที่ติดตาม ecosystem ของ Nous Research ครับ

