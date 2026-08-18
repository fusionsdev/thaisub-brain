---
videoId: "UVEjThz8DSo"
title: "One Memory, Many Agents? 🧠 Practical Hermes Guide (Hindsight & More)"
channel: "Wanderloots"
url: "https://www.youtube.com/watch?v=UVEjThz8DSo"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# One Memory, Many Agents? 🧠 Practical Hermes Guide (Hindsight & More)

> [!info] แหล่งที่มา
> Wanderloots · https://www.youtube.com/watch?v=UVEjThz8DSo

## 📝 สรุป

# สรุป: One Memory, Many Agents? 🧠 Practical Hermes Guide (Hindsight & More)

- **ช่อง:** Wanderloots · **ความยาว:** ~34 นาที · **ลิงก์:** https://www.youtube.com/watch?v=UVEjThz8DSo

## ประเด็นหลัก
- วิดีโอนี้สอนวิธีเชื่อมต่อเครื่องมือหน่วยความจำตัวเดียวชื่อ Hindsight เข้ากับ AI agents หลายตัว (Hermes, Codex, Claude Code, Gemini ฯลฯ) เพื่อให้ทุก agent ทำงานบนความทรงจำชุดเดียวกัน โดยไม่ต้องคัดลอกวางหรืออธิบายงานซ้ำ
- อธิบายแนวคิดหลักของระบบ: harness (โครงสร้างตัวแทน) กับโมเดลทำงานร่วมกันที่แต่ละเวิร์กสเตชัน และ Hindsight ทำหน้าที่เป็นสะพาน/สมุดบันทึกร่วมระหว่าง agents
- การตั้งค่าเริ่มต้น: สร้าง environment file เก็บ API key และรหัส control plane, ใช้ Docker Compose รัน Hindsight แบบต่อเนื่อง (restart unless stopped) และตั้งค่า LLM ผ่านการยืนยันตัวตนของ Codex ใน Docker volume แยก
- เลือกใช้ memory bank แบบ global user (ชื่อ Wanderloots) เหมาะกับผู้ใช้คนเดียว/นักพัฒนาเดี่ยว แทนที่จะแยก bank ต่อโปรเจกต์ เพราะ bank เป็นขอบเขตแข็งที่ไม่สามารถ query ข้ามกันได้
- ตั้งค่า bank configuration: extraction mode แบบ concise, mission statement, free form entities, entity labels (เช่น project, harness) ที่เชื่อมกับ tags เพื่อกรองความทรงจำแบบแยกอ่อนๆ ภายใน bank เดียว
- อธิบายการทำงานสามส่วนของ Hindsight: retain (จัดเก็บ/จดจำ), recall (ดึงบริบทกลับเข้าสู่ agent), reflect (ไตร่ตรองด้วยโมเดลที่แรงขึ้น) รวมถึง observations ที่รวมข้อเท็จจริงเป็นข้อสังเกตถาวร และ memory defense สำหรับปกปิดข้อมูลอ่อนไหว
- ติดตั้งระบบสำรองข้อมูลอัตโนมัติ (hindsight admin backup) และสาธิตการอัปเกรด Hindsight เป็นเวอร์ชัน 0.9 ที่มีฟีเจอร์ใหม่ knowledge pages และ knowledge base
- เชื่อมต่อ Hermes โดยเปลี่ยน memory provider จาก Memosyn เป็น Hindsight (โหมด local external) ตั้ง API key และ bank ID แล้วตรวจสอบด้วยคำสั่ง hermes memory status
- เชื่อมต่อ Codex ผ่านปลั๊กอิน Hindsight coding agents (คำสั่ง npx) พร้อม hooks อัตโนมัติสามอย่าง (initialize, recall, retain) และ MCP server ที่เพิ่มเครื่องมือจัดการ bank ให้ Codex
- ทดสอบการส่งต่อความทรงจำข้าม agent ทั้งสองทาง: ให้ Codex จำสีม่วงของโปรเจกต์ memory test แล้ว Hermes ตอบได้ทันที และให้ Hermes จำว่าชอบลีเมอร์ แล้ว Codex ดึงกลับมาได้ พร้อมการกรองความทรงจำด้วย tags ตาม harness
- knowledge pages คือการฉายภาพอัตโนมัติจากความทรงจำของ agents ที่อัปเดตตามเวลา ใช้สร้างแบบจำลองความคิดและสรุปโครงการ แต่ไม่ใช่ตัวแทนเอกสารที่มนุษย์ตรวจทานอย่าง LLM wiki ใน Obsidian
- สรุปทิ้งท้ายว่า ระบบหน่วยความจำอัตโนมัตินี้เป็นแค่ชั้นหนึ่งใน memory stack ยังต้องมีระบบความรู้แบบ human in the loop เพื่อต่อสู้กับข้อผิดพลาดและภาพหลอนของ AI ซึ่งจะพูดถึงในวิดีโอหน้า

## ความเห็นสรุป
วิดีโอนี้เป็นคู่มือภาคปฏิบัติที่ละเอียดและเป็นระบบ เหมาะกับผู้ใช้ AI agents หลายตัวที่อยากรวมศูนย์ความทรงจำไว้ที่เดียว แม้บางขั้นตอนจะซับซ้อน (Docker, การยืนยันตัวตน, hooks) แต่เจ้าของช่องอธิบายทีละขั้นอย่างชัดเจน และการสาธิตการส่งต่อความทรงจำระหว่าง Codex กับ Hermes แบบเรียลไทม์ทำให้เห็นคุณค่าของระบบได้จริง ข้อควรระวังคือคำบรรยายต้นฉบับเป็นแบบอัตโนมัติ ชื่อบางคำอาจเพี้ยน (เช่น Codex, Wanderloots, Memosyn) และเนื้อหาอิงเวอร์ชัน Hindsight 0.9 ซึ่งอาจมีการเปลี่ยนแปลงในภายหลัง

เสียงพากย์ไทย: ![[UVEjThz8DSo.mp3]]

