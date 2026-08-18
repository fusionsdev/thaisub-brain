---
videoId: "R1TNGOZAOZs"
title: "Improved AI Memory? 🧠 Full Hermes Tutorial (Mnemosyne & Hindsight)"
channel: "Wanderloots"
url: "https://www.youtube.com/watch?v=R1TNGOZAOZs"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Improved AI Memory? 🧠 Full Hermes Tutorial (Mnemosyne & Hindsight)

> [!info] แหล่งที่มา
> Wanderloots · https://www.youtube.com/watch?v=R1TNGOZAOZs

## 📝 สรุป

# สรุป: Improved AI Memory? 🧠 Full Hermes Tutorial (Mnemosyne & Hindsight)

- **ช่อง:** Wanderloots · **ความยาว:** ~26 นาที · **ลิงก์:** https://www.youtube.com/watch?v=R1TNGOZAOZs

## ประเด็นหลัก

- AI Agent ที่ไม่มีระบบความจำที่ดีจะลืมบริบทตลอดเวลา ทำให้เปลืองโทเค็นและเวลา โดยเฉพาะเมื่อใช้หลาย agent พร้อมกัน
- Memory stack ของ agentic AI ประกอบด้วย 3 ระดับ: world knowledge (Obsidian/LLM Wiki), built-in memory, และ external memory providers
- Built-in memory ของ Hermes (memory.md, user.md, soul.md + session search) ถูก inject เข้าทุก session — ดีแต่เปลืองโทเค็นถ้าใหญ่เกินไป
- Memory providers (Mnemosyne, Hindsight) เป็น external layer ที่ดึงข้อมูลเมื่อจำเป็นแทนที่จะ inject ทุกครั้ง — ช่วยให้บริบทกระชับ
- **Mnemosyne** — memory layer แบบเบา, zero-dependency, รันบน SQLite, เร็วระดับ sub-millisecond, ใช้ BEAM architecture, ไม่ต้องใช้ LLM, เหมาะสำหรับผู้ใช้ทั่วไป
- **Hindsight** — memory engine เต็มรูปแบบ, built-in ใน Hermes, มี reflect (ทบทวนด้วยเหตุผล), มี dashboard, ต้องรันเซิร์ฟเวอร์แยกและใช้ LLM
- การติดตั้ง Mnemosyne: ใช้ pipx ติดตั้งแยกจาก Hermes venv, ลิงก์เข้า plugins folder, รัน `hermes memory setup`, เลือก global scope
- การติดตั้ง Hindsight: รัน Docker container แยก, เชื่อมต่อกับ Ollama (local model), ตั้งค่าใน Hermes เป็น local external
- ทั้งสองระบบสามารถ export ข้อมูลระหว่างกันได้ — ไม่มีการล็อกอินกับผู้ให้บริการรายใด
- ขั้นต่อไป: เชื่อมต่อ agentic memory กับ Obsidian LLM Wiki เพื่อให้ agent ใช้เหตุผลกับความรู้ทั้งหมดของคุณ

## ความเห็นสรุป

วิดีโอนี้ให้คำแนะนำที่ใช้งานได้จริงในการติดตั้งระบบความจำให้ AI Agent โดย Callum อธิบายความแตกต่างระหว่าง memory layer และ memory engine อย่างชัดเจน Mnemosyne เหมาะสำหรับผู้ที่ต้องการความเร็วและความเรียบง่ายในเครื่องเดียว ส่วน Hindsight เหมาะสำหรับผู้ที่ต้องการฟีเจอร์ขั้นสูงอย่างการ reflect และ dashboard แบบเต็มรูปแบบ ทั้งสองตัวเลือกช่วยลดการเปลืองโทเค็นและทำให้ agent ทำงานได้ฉลาดขึ้นอย่างเห็นได้ชัด

เสียงพากย์ไทย: ![[R1TNGOZAOZs.mp3]]

