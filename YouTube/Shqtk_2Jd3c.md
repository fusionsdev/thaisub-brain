---
videoId: "Shqtk_2Jd3c"
title: "How to set up Herdr for multi-agent coding (full guide)"
channel: "Dave Ebbelaar"
url: "https://www.youtube.com/watch?v=Shqtk_2Jd3c"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-10-04"
tags: [thai-sub, youtube]
---

# How to set up Herdr for multi-agent coding (full guide)

> [!info] แหล่งที่มา
> Dave Ebbelaar · https://www.youtube.com/watch?v=Shqtk_2Jd3c

## 📝 สรุป

# สรุป: How to set up Herdr for multi-agent coding (full guide)

- **ช่อง:** Dave Ebbelaar · **ความยาว:** ~29 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Shqtk_2Jd3c

## ประเด็นหลัก

- Herdr คือเครื่องมือแบบ terminal multiplexer (คล้าย tmux) ออกแบบมาเพื่อจัดการ coding agent หลายตัวพร้อมกันในหน้าจอเดียว กำลังเป็นที่นิยมในชุมชนนักพัฒนา จน DHH พูดถึงในพอดแคสต์ของ Lex Fridman และใส่มาเป็นค่าเริ่มต้นใน Omachi Linux distribution
- จุดขายหลักคือ session แบบ persistent — ปิด terminal ไปแล้วเปิดใหม่ ทุกอย่าง (หน้าต่าง, tab, prompt, ประวัติ) ยังอยู่ครบ เหมาะกับการรัน Claude Code / Codex / Grok พร้อมกันหลายตัว
- โครงสร้างการใช้งาน: space = โปรเจกต์ (เทียบกับ project ใน Codex Desktop) ข้างในแยกเป็น tab และ panel ได้อิสระ สร้างได้โดย cd เข้าไปในโฟลเดอร์นั้นตรงๆ
- ต้องติดตั้ง integration ของแต่ละ agent harness ผ่านหน้า settings หรือคำสั่ง `herder integration install claude codex grok` เพื่อให้ agent แต่ละตัวขึ้นแสดงในส่วน agent ของ Herdr
- ปรับแต่งได้ทุกอย่างผ่าน `config.toml` — สี, ระยะห่าง, keyboard shortcut — และเคล็ดลับคือให้ AI agent อ่านไฟล์ config กับ documentation แล้วตั้งค่าให้เอง ไม่ต้องอ่านเอง
- ผู้จัดทำแนะนำเปลี่ยน prefix key (ค่าเริ่มต้น Ctrl+B แบบ tmux/Vim) มาเป็นปุ่มลัดแบบแอปปกติ เช่น Cmd+T สร้าง tab, Cmd+K กระโดดหา workspace พร้อมเสิร์ช และมีปุ่มลัดกระโดดไปหา agent ที่ทำงานเสร็จพร้อม ping แจ้งเตือน
- ฟีเจอร์เด่นสุดคือ agent delegation — ติดตั้ง skill ของ Herdr แบบ global แล้ว agent หนึ่งตัว (เช่น GPT-6 Astra เป็น orchestrator/reviewer) สั่งเปิด agent อีกตัว (เช่น Opus 5) ผ่าน Herdr CLI ได้เอง และ tab ต่างๆ สื่อสารกันผ่าน CLI ได้ด้วย
- เสริมช่องว่างที่ไม่มี IDE ด้วยเครื่องมือ terminal: Neovim (เรียกดูไฟล์), lazygit (ดู branch/diff/commit), zoxide + คำสั่ง zi (กระโดดหาโปรเจกต์ไวๆ)
- โบนัส: สร้าง custom MCP server ใน Glido (แอปพิมพ์ด้วยเสียงสำหรับนักพัฒนา) เพื่อสั่งเปิด agent ใน Herdr จากที่ไหนก็ได้โดยไม่ต้องเปิดแอปอื่น

## ความเห็นสรุป

วิดีโอนี้เป็นคู่มือปฏิบัติที่จับทางดีมากสำหรับนักพัฒนาที่อยากย้ายจาก desktop app (Claude Code / Codex) มาใช้งานหลาย agent ในเทอร์มินัลจอเดียว จุดแข็งคือเจ้าของวิดีโอแชร์ setup จริงทั้งหมดและสอนวิธีให้ AI agent ช่วยตั้งค่าแทนการอ่าน docs เอง แนะนำสำหรับคนที่ทำงานกับ coding agent หลายตัวหลายโมเดลเป็นประจำ แต่ต้องยอมรับความจริงว่ามี learning curve และต้องตั้งค่าเสริมด้วยเครื่องมืออื่นอีกหลายตัวก่อนจะใช้เป็นเครื่องมือหลักได้จริง

