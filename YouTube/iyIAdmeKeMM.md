---
videoId: "iyIAdmeKeMM"
title: "Stop Paying Claude for This. Use Jev Instead"
channel: "Leon van Zyl"
url: "https://www.youtube.com/watch?v=iyIAdmeKeMM"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-02"
tags: [thai-sub, youtube]
---

# Stop Paying Claude for This. Use Jev Instead

> [!info] แหล่งที่มา
> Leon van Zyl · https://www.youtube.com/watch?v=iyIAdmeKeMM

## 📝 สรุป

# สรุป: Stop Paying Claude for This. Use Jev Instead

- **ช่อง:** Leon van Zyl · **ความยาว:** ~16 นาที · **ลิงก์:** https://www.youtube.com/watch?v=iyIAdmeKeMM

## ประเด็นหลัก

- Jev จาก typesafe.ai ถูก overhype ว่าเป็น "Claude Killer" แต่จริง ๆ เขียนประโยคเต็มยังไม่ได้ — เป็น System 1 model (ตัดสินเร็ว ถูก) ไม่ใช่ System 2 (มี reasoning) อย่าง Claude/OpenAI
- Jev เก่ง 3 ประเภทคำถาม: Choice (เลือกจากตัวเลือก), Score (ให้คะแนนบนมาตรวัด), Null (ใช่/ไม่ใช่พร้อม confidence) — ตอบเป็นโครงสร้าง deterministic ที่การันตีเสมอ เหมาะ map กับ n8n/โค้ด
- ข้อจำกัด: ไม่มี reasoning แย่วิทย์/คณิต และ context window จิ๋วแค่ ~32,000 tokens
- ความคุ้มค่าคือต้นทุน: จำแนก 1 ล้านครั้ง Jev ~$21 เทียบ Sonnet 5 ~$1,500 และ Fable 5.1 ~$7,500
- confidence score (0-1) กลับมาทุกครั้ง — เขียน logic ได้เช่น ต่ำกว่า 0.75 ให้ส่งคนตรวจแทน
- สาธิตจริง: สร้าง issue ใหม่ใน GitHub → GitHub Action เรียก Jev → ติดป้าย enhancement/bug/documentation + เลือก agent (Fable งาน coding ขั้นสูง, Astra งาน 3D/spatial reasoning, Haiku เอกสาร) → โพสต์คอมเมนต์ input/response/confidence
- ผลจริง: issue "add a new emotion: scared" ถูกจำแนก enhancement (confidence 1.0) เลือก Astra (confidence 0.62 เพราะ description คลุมเครือ) ใช้ไม่ถึง 800 tokens
- เข้าถึงได้เลย: typesafe.ai (มี waitlist ช่วงอัด) หรือข้ามคิวผ่าน OpenRouter; สมัครใหม่มี free credits $5
- ติดตั้ง TypeSafe agent skill (ทางการ) ให้ Claude Code รู้จักวิธีเรียก Jev API
- ต่อยอด: label "ready" → "factory running" เพื่อให้ software factory หยิบ issue ไปทำจนเปิด pull request — workflow คล้าย diagram ของ Vercel เอง
- สปอนเซอร์ Decodo: web scraping API + MCP server, rotating IPs, JS rendering, ฟรี 2,000 credits/ปี โค้ด LEONVANZYL ลด 10%

## ความเห็นสรุป

คลิปนี้ให้มุมที่สมดุลระหว่าง hype กับความเป็นจริงของ Jev — ชื่อเรื่องจะโหดไปว่า "หยุดจ่ายเงิน Claude" แต่เนื้อในอธิบายครบว่า Jev เก่งเฉพาะงานจำแนกด่วนที่ไม่ต้องใช้ reasoning และถูกกว่ากันมหาศาลในการใช้งานจริง ส่วน demo ละเอียดดี ทำตามได้จริงตั้งแต่สร้าง API key จนต่อ software factory เป็นแนวทางที่นำไปใช้กับ repo หรือ workflow อื่นได้กว้าง

เสียงพากย์ไทย: ![[iyIAdmeKeMM.mp3]]

