---
videoId: "F6PYMo6VAFs"
title: "Day 1A: Intro to AI Agents — Complete Beginner Breakdown (Google x Kaggle Intensive)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=F6PYMo6VAFs"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 1A: Intro to AI Agents — Complete Beginner Breakdown (Google x Kaggle Intensive)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=F6PYMo6VAFs

## 📝 สรุป

# สรุป: Day 1A: Intro to AI Agents — Complete Beginner Breakdown (Google x Kaggle Intensive)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~23 นาที · **ลิงก์:** https://www.youtube.com/watch?v=F6PYMo6VAFs

## ประเด็นหลัก

- งาน Day 1 มี 2 ขั้นเตรียม: ฟังพอดแคสต์สรุปเนื้อหา และอ่าน white paper เรื่อง Introduction to Agents แต่ถ้ายังไม่ได้ทำก็ไม่กระทบการทำ codelab
- ต้องยืนยันเบอร์โทรศัพท์ในบัญชี Kaggle ก่อน ไม่อย่างนั้นจะรันโค้ดใน codelab ไม่ได้เลย
- codelab มี 2 แบบฝึกหัด: สร้าง agent ตัวแรก และสร้างระบบ multi-agent — วิดีโอนี้โฟกัสข้อแรก ส่วน multi-agent แยกไปวิดีโอถัดไป
- ADK (Agent Development Kit) ขับเคลื่อนด้วย Gemini และให้ agent ใช้ Google Search ตอบคำถามด้วยข้อมูลล่าสุดได้
- codelab ที่สองยังสอนการสร้างทีม agent เฉพาะทาง และ architectural patterns แบบ sequential, parallel และ loop
- ต้องกด "Copy & Edit" เพื่อสร้างสำเนา Kaggle Notebook ที่แก้ไขได้ก่อนเริ่มทำงาน
- API key สร้างใน Google AI Studio แนะนำให้สร้าง project ใหม่เองเพื่อความคุ้นเคย และห้ามแชร์ key ให้ใครเด็ดขาด
- secret ใน Notebook เป็นแบบ case-sensitive และต้องติ๊ก attach ให้ถูกต้อง ไม่งั้นขั้นตอน authenticate จะ error
- retry option จัดการ transient error อย่าง rate limit ด้วย exponential backoff (5 ครั้ง, ตัวคูณ 7, delay เริ่มต้น 1 วินาที)
- ความต่างหลัก: model ตอบกลับด้วยข้อความ แต่ agent คิด-ลงมือ-สังเกตผล (think, act, observe) เหมือน Siri
- agent ประกอบด้วย name, description, model (Gemini 2.5 Flash), instruction และ tools (Google Search)
- runner ทำหน้าที่เป็น orchestrator จัดการ session และการตอบกลับของ agent
- ขั้นสุดท้าย generate sample agent แล้วรันผ่าน web interface ที่เปิดเป็นหน้าแชทคุยกับ agent ได้

## ความเห็นสรุป

วิดีโอนี้เหมาะกับผู้เริ่มต้นมากครับ เพราะอธิบายตั้งแต่พื้นฐานว่า agent ต่างจาก model อย่างไร แล้วพาทำทีละขั้นจนได้ agent ตัวแรกที่ค้นข้อมูลจริงผ่าน Google Search ครับ แม้คำบรรยายต้นฉบับจะถอดเสียงเพี้ยนหลายจุด แต่เนื้อหาหลักยังติดตามได้ครบและทำตามได้จริงครับ

เสียงพากย์ไทย: ![[F6PYMo6VAFs.mp3]]

