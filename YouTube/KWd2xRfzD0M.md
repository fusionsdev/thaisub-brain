---
videoId: "KWd2xRfzD0M"
title: "Testing Reverse Engineer Anything: Is Software Really Done?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=KWd2xRfzD0M"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-10-20"
tags: [thai-sub, youtube]
---

# Testing Reverse Engineer Anything: Is Software Really Done?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=KWd2xRfzD0M

## 📝 สรุป

# สรุป: Testing Reverse Engineer Anything: Is Software Really Done?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~15 นาที · **ลิงก์:** https://www.youtube.com/watch?v=KWd2xRfzD0M

## ประเด็นหลัก

- REA (Reverse Engineer Anything) คือโปรเจกต์ GitHub จาก Moruto ที่มี 150K+ ดาว — รวมเครื่องมือ MCP และ CLI เพื่อให้ AI agent วิเคราะห์ซอฟต์แวร์แบบย้อนกลับได้
- เครื่องมือหลักที่ REA ใช้คือ Hopper และ Ghidra สำหรับ decompile, Playwright สำหรับวิเคราะห์เว็บไซต์, และ parser สำหรับ JavaScript/Electron
- จุดเริ่มต้นกระแสมาจาก Matthew Burman โพสต์ "software is done" ที่มียอดวิว 3.5 ล้านครั้ง
- Tonbi ทดลองใช้ REA ผ่าน Hermes Agent (รันด้วย Claude Opus 5.5) เพื่อวิเคราะห์แอป Loom Recorder
- ข้อจำกัด: REA วิเคราะห์แอปขนาดใหญ่ไม่ได้ (Loom ตัวเต็ม 532MB) แต่วิเคราะห์เฉพาะโค้ดของแอปได้
- ผลการวิเคราะห์พบว่า Loom ใช้ 35 หน้าต่างที่ถูกรวมให้ดูเหมือน HUD เดียว และมี 55 unnamed channels
- การ decompile pause/resume handler ใน native recorder ของ Loom ด้วย Ghidra ได้ข้อมูลสำคัญเพื่อนำมาเปรียบเทียบกับ Recordly
- Tonbi นำข้อมูลที่ได้มาแก้ไขโปรแกรมบันทึกหน้าจอที่เขาพัฒนาเอง (Garage Studio ซึ่งใช้ Recordly เป็นฐาน)
- ผลลัพธ์: แก้ปัญหาลาก HUD ไม่ได้ + เครื่องค้างบ่อย + ปิดด้วยปุ่ม X ไม่ได้ — ทั้งหมดทำงานได้ปกติแล้ว
- แผนต่อไป: พัฒนาโปรแกรมต่อให้เป็น agentic มากขึ้น อาจ integrate Hermes Agent เข้าไปในโปรแกรมตัดต่อวิดีโอ

## ความเห็นสรุป

REA ไม่ใช่ "ไม้กายสิทธิ์" ที่จะลอกซอฟต์แวร์ทั้งตัวได้ แต่เป็นเครื่องมือที่ช่วยให้ agent ได้ "เบาะแส" ว่าซอฟต์แวร์ต้นฉบับทำงานอย่างไร แล้วนำมาประยุกต์ใช้กับโปรเจกต์ของเราได้จริง Tonbi พิสูจน์ให้เห็นแล้วว่าวิธีนี้ใช้ได้ผล — แก้บั๊กที่ค้างมานานหลาย build ได้ในครั้งเดียวด้วยข้อมูลจาก REA

