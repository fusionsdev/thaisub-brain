---
videoId: "oQdkFPhqaGk"
title: "Complete Guide to building an AI Trading Bot with Claude for Beginners"
channel: "Ray Fu"
url: "https://www.youtube.com/watch?v=oQdkFPhqaGk"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-25"
tags: [thai-sub, youtube]
---

# Complete Guide to building an AI Trading Bot with Claude for Beginners

> [!info] แหล่งที่มา
> Ray Fu · https://www.youtube.com/watch?v=oQdkFPhqaGk

## 📝 สรุป

# สรุป: Complete Guide to building an AI Trading Bot with Claude for Beginners

- **ช่อง:** Ray Fu · **ความยาว:** ~14 นาที · **แหล่ง:** https://www.youtube.com/watch?v=oQdkFPhqaGk

## ประเด็นหลัก

- สร้างบอทเทรดหุ้นอัตโนมัติตั้งแต่ศูนย์ **โดยไม่ต้องมีพื้นฐานเทคนิค** — ทุกอย่างทำผ่านการคุยกับ Claude
- เครื่องมือ: **Claude Desktop + Claude Code**, โบรกเกอร์ **Alpaca** (paper trading เงินจำลอง $50,000), **Alpaca MCP** เชื่อม Claude กับ Alpaca
- คุณค่าของบอท: แก้จุดอ่อน "การลงมือ" ของเทรดเดอร์ — ไม่ลังเล ไม่ลืม ไม่มีอารมณ์ ทำงาน 24/7
- กลยุทธ์สำหรับมือใหม่: **Moving Average Crossover** — MA เส้น fast (20 วัน) ตัดขึ้นเหนือ MA เส้น slow (50 วัน) = ซื้อ; ตัดลง = ขาย คือคณิตศาสตร์ล้วน ไม่มีการเดา
- ข้อจำกัดของกลยุทธ์: เก่งในตลาดที่มีแนวโน้มชัด แต่ในตลาดออกข้างจะเกิดไม้ขาดทุนเล็ก ๆ ต่อเนื่อง — ไม่มีกลยุทธ์ใดชนะทุกครั้ง
- ข้อมูลราคาดึงจาก **YFinance (Yahoo Finance)** ย้อนหลัง 100 วัน, API keys เก็บในไฟล์ **.env**
- ทำอัตโนมัติ: ให้ Claude ตั้งรันวันจันทร์–ศุกร์ เวลา 9:30 EST พร้อมตลาดเปิด พร้อม log ทุกการทำงาน
- เงื่อนไข: คอมพิวเตอร์ต้องเปิดค้างไว้ และควรมี Python + Node.js ติดตั้งไว้
- ทุกอย่างทดสอบบน paper trading — ไม่มีความเสี่ยงเงินจริง (ผู้สอนย้ำว่าไม่ใช่คำแนะนำการเงิน)

## ความเห็นสรุป

คลิปนี้เหมาะกับคนที่อยากเห็น "AI agent ทำงานจริงจัง" มากกว่านักเทรดจริงจัง — มันโชว์พลังของการสั่งงานด้วยภาษาธรรมชาติได้ชัดเจนมาก: ตั้งบัญชี เชื่อม MCP สร้างโค้ดบอท ตั้งเวลารันอัตโนมัติ จบครบวงจรใน 14 นาที ข้อควรระวังคือกลยุทธ์ crossover เป็นเพียงจุดเริ่มต้น และการที่บอท "ทำงานได้" ไม่เท่ากับ "ทำกำไรได้" — ควรทดสอบด้วย paper trading ยาว ๆ ก่อนใช้เงินจริงเสมอ

เสียงพากย์ไทย: ![[oQdkFPhqaGk.mp3]]

