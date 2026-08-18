---
videoId: "N2Ogvx_U8uM"
title: "Claude Can Use Your Apps Now"
channel: "Leon van Zyl"
url: "https://www.youtube.com/watch?v=N2Ogvx_U8uM"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Claude Can Use Your Apps Now

> [!info] แหล่งที่มา
> Leon van Zyl · https://www.youtube.com/watch?v=N2Ogvx_U8uM

## 📝 สรุป

# สรุป: Claude Can Use Your Apps Now

- **ช่อง:** Leon van Zyl · **ความยาว:** ~28 นาที · **ลิงก์:** https://www.youtube.com/watch?v=N2Ogvx_U8uM

## ประเด็นหลัก

- Claude connectors ที่ติดตั้งมาล่วงหน้าเชื่อม Claude กับ GitHub, Gmail, Drive, Motion และแอปอื่น ๆ ได้ แต่เราสร้างตัวเชื่อมต่อแบบกำหนดเองสำหรับแอปของตัวเองได้ โดยยกตัวอย่าง PulseBooks แอปทำบัญชีของผู้บรรยาย ที่ให้ Claude สร้างรายการค่าใช้จ่ายจากรูปใบเสร็จได้แทนผู้ใช้
- เริ่มจากใช้สกิล start-app ตั้งโปรเจกต์ใหม่ พร้อมให้ agent สร้างแอป Trello clone ที่รองรับองค์กร ทีม บทบาท คำเชิญ และการลากการ์ดบนกระดาน Kanban
- ขั้นตอนสำคัญ: ให้ agent สร้างแพลนระดับสูงก่อน แล้วขยายเป็น implementation plan รายละเอียดที่แยกเป็นไฟล์ฟีเจอร์แต่ละตัวพร้อม acceptance criteria ก่อนลงมือ implement เพื่อลดความเสี่ยงที่ฟีเจอร์จะตกหล่น
- ติดตั้ง Playwright MCP server เพื่อให้ agent เปิดเบราว์เซอร์ทดสอบแอปจริงแบบ end-to-end พร้อมตั้งค่าไฟล์ AGENTS.md/CLAUDE.md ให้ทดสอบและใช้ข้อมูลชุดเดิมซ้ำ (test-data.json)
- ดีพลอยแอปขึ้น production ด้วย GitHub + Vercel และ Neon serverless Postgres พร้อมวิธีแก้ปัญหาการสมัครสมาชิกล้มเหลวผ่าน Vercel logs ซึ่งเกิดจากการลืมรัน database migration
- เปิดเผยแอปให้ AI เข้าถึงโดยสร้าง remote MCP server (ที่ domain/mcp) เปิดเผย tools เช่น create expense ให้ agent เรียกใช้โดยไม่ต้องผ่าน UI
- ใช้ Better Auth + โปรโตคอล OAuth เพื่อให้ agent ยืนยันตัวตนและทำงานแทนผู้ใช้จริง โดยเก็บ token ปลอดภัยไว้ในฝั่ง client และเพิกถอนสิทธิ์ได้ทุกเมื่อ
- สร้าง Claude connector ชื่อ Lanes เชื่อมต่อกับ Claude web, Claude desktop app และ Claude code ได้ทั้งหมด พร้อมควบคุมสิทธิ์ของแต่ละ tool (ต้องอนุมัติ / บล็อก / อนุมัติอัตโนมัติ)
- ทดสอบจริง: สร้างงานใหม่ใน Lanes, assign ให้ตัวเอง, เปลี่ยนสถานะเป็น doing, และแสดงรายการงาน — ระบบรู้ว่าการเปลี่ยนแปลงเกิดขึ้นภายใต้ชื่อผู้ใช้ของ Leon
- ผู้บรรยายแนะนำคอร์สฟรีเรื่อง RAM framework และคอมมูนิตี้ Agentic Labs พร้อม Masterclass การสร้างแอป SaaS เต็มรูปแบบ

## ความเห็นสรุป

คลิปนี้เป็นบทช่วยสอนที่ครบวงจรและทำตามได้จริง ตั้งแต่การสร้างแอปด้วย coding agent ไปจนถึงการเปิดเผยแอปให้ AI agent เข้าถึงผ่าน MCP server และ OAuth อย่างปลอดภัย จุดเด่นคือการอธิบาย "ทำไม" ทุกขั้นตอน เช่น การขยายแพลนก่อน implement และการใช้โปรโตคอล OAuth เพื่อให้ agent ทำงานแทนผู้ใช้โดยรู้ตัวตนผู้ใช้จริง ๆ เนื้อหามีประโยชน์มากสำหรับนักพัฒนาที่อยาก "AI-enable" แอปของตัวเอง

เสียงพากย์ไทย: ![[N2Ogvx_U8uM.mp3]]

