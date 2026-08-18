---
videoId: "TTSPDNUinek"
title: "I Built an AI Content Studio with 5 Hermes Agents (Step-by-Step Guide)"
channel: "Komputer Mechanic"
url: "https://www.youtube.com/watch?v=TTSPDNUinek"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# I Built an AI Content Studio with 5 Hermes Agents (Step-by-Step Guide)

> [!info] แหล่งที่มา
> Komputer Mechanic · https://www.youtube.com/watch?v=TTSPDNUinek

## 📝 สรุป

# สรุป: I Built an AI Content Studio with 5 Hermes Agents (Step-by-Step Guide)

- **ช่อง:** Komputer Mechanic · **ความยาว:** ~115 นาที · **ลิงก์:** https://www.youtube.com/watch?v=TTSPDNUinek

## ประเด็นหลัก

- ลาร์รี (Larry) จากช่อง Komputer Mechanic สร้าง "Cadence" ซึ่งเป็นระบบอัตโนมัติจัดการงานคอนเทนต์ครบวงจร (content operations autopilot) บน Hermes Agents โดยมีเอเจนต์ 5 ตัวทำงานร่วมกัน
- เอเจนต์ทั้ง 5 ตัว ได้แก่ **orchestrator** (ผู้ประสานงานหลัก รับคำสั่งผ่าน Telegram) **Atlas/Scout** (นักวิจัยและเสนอไอเดีย) **Vera/Scribe** (นักเขียนสไลด์ แคปชัน แฮชแท็ก) **Kite/Dev** (นักออกแบบ + นักพัฒนา สร้างแดชบอร์ด) และ **Orion/Rich** (นักเผยแพร่โพสต์)
- ผู้ชมสามารถสร้างตามได้จริงตั้งแต่ศูนย์: เช่า VPS (แนะนำ Racknerd ~$35/ปี หรือ Contabo ~$8/เดือน) ติดตั้ง Ubuntu แล้วติดตั้ง Hermes พร้อมผูกบัญชี Nous Research และเลือกโมเดล AI (เช่น OpenAI Codex ผ่านแผน ChatGPT Plus/Pro, Grok ผ่านบัญชี X, หรือ OpenRouter)
- สร้าง Telegram group พร้อม topics แยกช่องต่อเอเจนต์ (orchestrator / Kite / studio) สร้างบอทผ่าน BotFather ใช้ User Info Bot หา user ID และตั้งค่าการผูกช่องกับเอเจนต์ (topic-lane binding) เพื่อให้แต่ละเอเจนต์ฟังเฉพาะช่องของตัวเอง
- สร้างโปรไฟล์เอเจนต์แบบ persistent พร้อมไฟล์ soul.md กำหนดบทบาท หน่วยความจำเฉพาะ (dedicated memory) และขอบเขตบทบาท (role boundaries) เพื่อป้องกันไม่ให้เอเจนต์ก้าวก่ายงานกัน
- สร้างฐานข้อมูลบันทึกการทำงานของเอเจนต์ด้วย **SQLite** — เอเจนต์ทุกตัวบันทึกชื่อ งานที่ทำ โมเดล AI และ timestamp ลงตาราง cadence runs ก่อนตอบกลับทุกครั้ง เพื่อให้แดชบอร์ดแสดงเมตริกจริง ไม่ใช่ค่าฮาร์ดโค้ด
- จุดเด่นของระบบคือสไลด์ carousel ถูกสร้างเป็นไฟล์ **HTML** แล้วเรนเดอร์เป็นภาพผ่าน headless browser (Chromium) ทำให้แก้ไขข้อความ ดีไซน์ ได้ไม่จำกัดโดยไม่เสียค่าใช้จ่ายต่อสไลด์ (ต่างจากโมเดลสร้างภาพที่คิดเงินทุก API call)
- เชื่อมต่อ API keys สามตัว: **Perplexity** (วิจัยเชิงลึก), **ImgBB** (พื้นที่เก็บภาพตัวกลาง) และ **Buffer** (ส่งโพสต์ไปยังโซเชียลมีเดีย) — ขั้นตอนการโพสต์: Cadence → ImgBB → Buffer → Instagram พร้อมระบบยืนยันก่อนโพสต์ทุกครั้ง
- รักษาความปลอดภัยด้วย **SSH tunneling** ในการเข้าถึงแดชบอร์ดช่วงแรก จากนั้นติดตั้ง **Tailscale** เพื่อเข้าถึงแดชบอร์ดจากอุปกรณ์ใดก็ได้ที่ผูกบัญชี โดยไม่เปิดให้อินเทอร์เน็ตสาธารณะ
- แดชบอร์ดมีแท็บครบ: ideas (สร้าง/โปรโมตไอเดีย), studio (fine-tune สไลด์, แปลง carousel เป็น reel), publish, templates (เทมเพลต HTML 50+ แบบ), agents (heat map + workload), calendar, configuration และ docs — พร้อมรีโมตคอนโทรลผ่าน Telegram (คำสั่ง /ideas, /promote)
- ระหว่างทางมีการแก้ปัญหาจริงที่พบ เช่น error "failed to connect to bus" ตอนรีสตาร์ท gateway, เซิร์ฟเวอร์ทดสอบลบข้อมูลในฐานข้อมูลโปรดักชัน, ชื่อเทมเพลตไม่ตรงกันระหว่างแดชบอร์ดกับ Telegram และมีตัวติดตั้งอัตโนมัติ (auto installer) สำหรับสมาชิกที่ไม่อยาก build เอง 4-5 ชั่วโมง

## ความเห็นสรุป

วิดีโอนี้เป็นบทช่วยสอนแบบ step-by-step ที่ละเอียดมาก ครอบคลุมทั้งฮาร์ดแวร์ (VPS) ซอฟต์แวร์ (Hermes, Telegram, SQLite, Python) และการออกแบบระบบ multi-agent จริง เนื้อหาเน้นการปฏิบัติจริง มีการโชว์เดโม่สดและแก้ไขข้อผิดพลาดระหว่าง build ทำให้เห็นกระบวนการคิดและแนวทางแก้ปัญหาที่นำไปใช้ต่อได้จริง จุดที่คุ้มค่าที่สุดคือแนวคิด "สไลด์เป็น HTML แล้วเรนเดอร์ด้วย headless browser" ซึ่งช่วยประหยัดต้นทุนได้มาก และการแยกบทบาท/หน่วยความจำของเอเจนต์อย่างเป็นระบบ

เสียงพากย์ไทย: ![[TTSPDNUinek.mp3]]

