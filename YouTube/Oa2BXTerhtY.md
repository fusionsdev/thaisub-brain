---
videoId: "Oa2BXTerhtY"
title: "Exploring Herdr: The Best Agent Multiplexer?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=Oa2BXTerhtY"
published: "2026-07-24"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Exploring Herdr: The Best Agent Multiplexer?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=Oa2BXTerhtY

## 📝 สรุป

# สรุป: Exploring Herdr: The Best Agent Multiplexer?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~17.5 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Oa2BXTerhtY

## ประเด็นหลัก

- **Herdr คือ agent multiplexer แบบโอเพนซอร์ส** ที่ออกแบบมาสำหรับ coding agent โดยเฉพาะ คล้ายกับที่ tmux เป็นกับเทอร์มินัล — เป็น Rust binary ตัวเดียวที่รัน agent ใน persistent PTY
- **สถาปัตยกรรมแบบ client/server:** server รันเบื้องหลังและเป็นเจ้าของโพรเซสทั้งหมด ส่วน client คือ UI ที่ผู้ใช้เชื่อมต่อเข้าไป การแยกนี้ทำให้เซสชันคงอยู่แม้ปิดเทอร์มินัล
- **การติดตั้งง่ายและรวดเร็ว** บน WSL/Linux/macOS — แค่รันคำสั่งเดียว ส่วน Windows ยังอยู่ในสถานะพรีวิวเบต้า
- **เน้นการใช้เมาส์เป็นหลัก** UI สะอาดตา ปรับแต่ง pane, theme, การแจ้งเตือน และ integration กับ agent ต่าง ๆ ได้ง่าย
- **Integrations** รองรับ Codex, Claude, OpenCode, Hermes, Grok และอื่น ๆ — ทำให้ agent รายงานสถานะได้โดยตรง
- **Socket API** เป็นฟีเจอร์เด่น — ช่วยให้ agent หนึ่งสามารถอ่านสถานะของ agent อื่น ๆ และสั่งงานได้ เช่น Hermes agent สามารถตอบคำถามที่ Codex ถาม หรือสั่งเปิดเซสชัน Claude ใหม่ได้
- **การคงอยู่ (persistence):** ปิดเทอร์มินัลแล้วกลับมาด้วยคำสั่ง `her` เซสชันทั้งหมดยังอยู่ครบ — สามารถ SSH เข้ามาจากมือถือแล้วรันต่อได้
- **Plugins marketplace** บน herdr.dev มีปลั๊กอินจากชุมชนกว่า 307 ตัว เช่น Herdr Flock ที่แสดง agent ในรูปแบบตัวละครน่ารัก ๆ
- **การเปลี่ยนลิขสิทธิ์เป็น Apache 2.0** ทำให้เป็นโอเพนซอร์สโดยสมบูรณ์ ใครก็ใช้และต่อยอดได้
- **เหมาะกับ** ผู้ที่รัน agent หลายตัวและหลายโปรเจกต์พร้อมกัน หรือทำงานยาว ๆ — ไม่จำเป็นถ้ามีแค่ agent เดียว เซสชันสั้น ๆ

## ความเห็นสรุป

Herdr เป็นเครื่องมือที่ตอบโจทย์ความต้องการจริงของนักพัฒนาที่ใช้ coding agent หลายตัวพร้อมกัน ความสามารถในการคงอยู่ของเซสชันและการอนุญาตให้ agent ควบคุม agent อื่นผ่าน socket API เป็นจุดเด่นที่ทำให้มันแตกต่างจากเครื่องมืออื่น ๆ เจ้าของช่องมาด้วยความสงสัยในตอนแรก แต่หลังลองใช้แล้วก็พบว่าชอบและจะใช้ต่อไปในอนาคตครับ

เสียงพากย์ไทย: ![[Oa2BXTerhtY.mp3]]
