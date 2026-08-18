---
videoId: "-8yZx5pny1s"
title: "Herdr Multiplexer: The Agent OS that Runs All Coding Agents from One Terminal"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=-8yZx5pny1s"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Herdr Multiplexer: The Agent OS that Runs All Coding Agents from One Terminal

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=-8yZx5pny1s

## 📝 สรุป

# สรุป: Herdr Multiplexer: The Agent OS that Runs All Coding Agents from One Terminal

- **ช่อง:** DevsKingdom · **ความยาว:** ~9 นาที · **ลิงก์:** https://www.youtube.com/watch?v=-8yZx5pny1s

## ประเด็นหลัก

- Herdr คือโปรเจกต์โอเพนซอร์สแบบ agent multiplexer ที่ให้รันเอเจนต์เขียนโค้ดทั้งหมดไว้ในเทอร์มินัลเดียว
- การติดตั้งง่ายมาก ใช้สคริปต์เดียวจบ และตัวโปรเจกต์บน GitHub มีดาวเกือบ 16K
- ภายใน workspace (พื้นที่ทำงาน) หนึ่งสามารถเปิดเอเจนต์ได้หลายตัว และเอเจนต์ทุกตัวคุยกันได้
- UI แบ่งเป็น workspace ทางซ้าย และ panes (แผงย่อย) ทางขวา แต่ละแท็บ/แต่ละ pane ทำงานของตัวเอง
- รองรับการแยก pane แบบเดียวกับ tmux ด้วยคีย์ลัด Control B แล้วกด V เพื่อแยกไปทางขวา กด exit เพื่อปิด
- สั่งรันเอเจนต์ใน pane ที่ต้องการผ่านคำสั่ง hermes pane run พร้อมระบุ workspace ID, pane ID และพรอมป์ต
- ดูภาพรวม pane ทั้งหมดด้วย Control B แล้วกด G เพื่อดู pane ID
- รอให้เอเจนต์ในอีก pane เสร็จสิ้นก่อนรันต่อได้ ผ่าน socket API และคำสั่งแบบ wait for agent
- รองรับเอเจนต์หลากหลาย เช่น Claude, Codex, Claude Code, Hermes, Kimi, Open Code, Kilo และอื่น ๆ
- การติดตั้งเอเจนต์แต่ละตัวทำผ่านคำสั่ง herdr integration install เช่น ติดตั้ง Claude hook หรือ Codex hook
- มีเอกสารครบทั้ง CLI reference, socket API, quick start และส่วน agent พร้อมคีย์ลัดทั้งหมด

## ความเห็นสรุป

วิดีโอนี้สาธิต Herdr ได้กระชับและเห็นภาพชัด เหมาะสำหรับคนที่ใช้เอเจนต์เขียนโค้ดหลายตัวและอยากรวมทุกอย่างไว้ในที่เดียว จุดเด่นคือความง่ายในการติดตั้ง การสั่งงานเอเจนต์ข้าม pane ได้ และการที่เอเจนต์คุยกันได้ภายในเทอร์มินัลเดียว ข้อเสียคือคำบรรยายอัตโนมัติทำให้ชื่อบางอย่าง (repo, เว็บไซต์, รายชื่อเอเจนต์บางตัว) เพี้ยนไปบ้าง แต่เนื้อหาหลักยังเข้าใจได้ครบถ้วน

เสียงพากย์ไทย: ![[-8yZx5pny1s.mp3]]

