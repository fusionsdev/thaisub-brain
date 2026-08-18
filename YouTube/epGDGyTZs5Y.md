---
videoId: "epGDGyTZs5Y"
title: "I Gave Claude Permission to Do Real Work for Me"
channel: "Leon van Zyl"
url: "https://www.youtube.com/watch?v=epGDGyTZs5Y"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# I Gave Claude Permission to Do Real Work for Me

> [!info] แหล่งที่มา
> Leon van Zyl · https://www.youtube.com/watch?v=epGDGyTZs5Y

## 📝 สรุป

# สรุป: I Gave Claude Permission to Do Real Work for Me
- **ช่อง:** Leon van Zyl · **ความยาว:** ~25 นาที (1475 วินาที) · **ลิงก์:** https://www.youtube.com/watch?v=epGDGyTZs5Y

## ประเด็นหลัก
- ยุคของแชตบอตที่สรุปหรือค้นหาข้อมูลได้อย่างเดียวนั้นจบลงแล้ว ผู้คนคาดหวัง agent ที่ทำงานแทนตนและจัดการงานซับซ้อนได้
- สถาปัตยกรรมของ agent ที่ดีมีสามส่วน: สมอง (โมเดล), tools (เครื่องมือ) และ permissions layer (ชั้นสิทธิ์การเข้าถึง)
- ตัวอย่างจริง: แอปจัดการสัญญา NDA ที่ agent สร้างร่าง ส่งให้คู่สัญญา ติดตามสถานะ และให้ผู้ใช้ตรวจสอบก่อนลงมือเสมอ
- เทคโนโลยีที่ใช้: โมเดล Claude (Opus 5), Claude Agent SDK, Claude Code, MCP server และ DocuSign IAM
- DocuSign IAM เป็นทั้งระบบจัดเก็บข้อมูลหลัก (system of record) และระบบลงมือปฏิบัติ (system of action) สำหรับสัญญาทั้งหมด
- ติดตั้งสอง dependency หลักก่อนเริ่ม: Playwright MCP server (ให้ agent ควบคุมเบราว์เซอร์และเทสต์แอป) และ start an app skill (กำหนดแนวทาง tech stack)
- ใช้โหมดวางแผน (planning mode) สร้างแอป Agreement Agent โดย agent ถามคำถามเพื่อความกระจ่าง เช่น ฐานข้อมูล ระบบ auth และโครงหน้าจอ ก่อนลงมือสร้าง
- เชื่อมต่อ DocuSign ผ่าน developer portal: สร้าง integration key, secret key และตั้งค่า redirect URI ที่ /api/docusign/callback
- สร้าง NDA template และ workflow ใน DocuSign: กำหนด role เป็น internal approver และ counterparty พร้อมฟิลด์ลายเซ็น ชื่อ และวันที่
- agent มีสิทธิ์เท่ากับผู้ใช้ที่ล็อกอินอยู่เท่านั้น และจะขออนุมัติจากมนุษย์ก่อนดำเนินการสำคัญทุกครั้ง
- ทดสอบจริง: ส่ง NDA ให้ Jane, เซ็นเอกสาร, แล้วสอบถามสถานะได้ถูกต้องตามลำดับการเซ็นที่ตั้งไว้
- ซอร์สโค้ดของโปรเจกต์ดาวน์โหลดฟรีจาก GitHub (ลิงก์ในคำอธิบายวิดีโอ) และวิดีโอนี้ได้รับการสนับสนุนจาก DocuSign

## ความเห็นสรุป
วิดีโอนี้เป็นบทช่วยสอนแบบลงมือทำจริงที่แสดงภาพรวมการสร้างแอปที่ให้ AI agent เป็นศูนย์กลางได้อย่างเป็นรูปธรรม ตั้งแต่แนวคิดสถาปัตยกรรม การเชื่อมต่อเครื่องมือภายนอกผ่าน MCP ไปจนถึงการทดสอบงานจริงครบวงจร จุดเด่นคือการเน้นว่า agent ควรทำงานร่วมกับมนุษย์ ไม่ใช่แทนที่ โดยขออนุมัติและตรวจสอบก่อนลงมือทุกครั้ง เหมาะสำหรับผู้ที่อยากเริ่มสร้างแอปแบบ agent-ready ด้วย Claude และ DocuSign

เสียงพากย์ไทย: ![[epGDGyTZs5Y.mp3]]

