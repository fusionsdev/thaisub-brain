---
videoId: "3RoK0rrOHCA"
title: "Is Hermes Bot Mode Worth It? 🧠 My Best Practices (So Far)"
channel: "Wanderloots"
url: "https://www.youtube.com/watch?v=3RoK0rrOHCA"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-08"
tags: [thai-sub, youtube]
---

# Is Hermes Bot Mode Worth It? 🧠 My Best Practices (So Far)

> [!info] แหล่งที่มา
> Wanderloots · https://www.youtube.com/watch?v=3RoK0rrOHCA

## 📝 สรุป

# สรุปภาษาไทย — Is Hermes Bot Mode Worth It? 🧠 My Best Practices (So Far)

> **ที่มา:** [YouTube — Wanderloots](https://www.youtube.com/watch?v=3RoK0rrOHCA) · เผยแพร่ 6 ก.ย. 2026 · ~35 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Wanderloots*

## วิดีโอนี้เกี่ยวกับอะไร
Callum (Wanderloots) ทดสอบฟีเจอร์ **bot mode** ใหม่ของ Hermes Agent ที่ทำให้เอเจนต์เฉพาะทางหลายตัวสื่อสารถึงกันได้ (agent-to-agent) โดยประกอบทีมงานวิจัย 3 ตัวแล้วรันงานวิจัยจริง 1 ชิ้นเพื่อดูข้อดีข้อเสีย

## ประเด็นหลัก

1. **Bot = Profile** — bot mode ไม่ใช่ primitive ใหม่ แค่ทำให้โปรไฟล์หลายตัวทำงานพร้อมกันและแท็กเรียกกันได้ (@mention) แต่ละ bot มี chat ถาวรของตัวเอง (พิมพ์ /new = compact ไม่ใช่สร้างใหม่)
2. **ทีมตัวอย่าง:** orchestrator (ประสานงาน/คุมคุณภาพ), researcher (สืบค้น+อ้างอิง), librarian (จัดเก็บลง LLM wiki) — ระบุหน้าที่ผ่าน description แล้ว Hermes สร้าง **soul.md อัตโนมัติ** ได้ หรือแก้เองเพื่อใส่ "team protocol" เช่น ห้ามทำงานข้ามบทบาท
3. **ประสิทธิภาพคือหัวใจ (ส่วนสำคัญที่สุด):** ตัดสิทธิ์/tools ที่ไม่จำเป็นออกทีละตัว — ตัวอย่างเด่น: researcher เคยวน task delegation 6 ครั้ง = เสียเวลา 20 นาที หลังตัด tools ทีมเร็วขึ้นมาก
4. **สมอง:** เลือกโมเดลแยกตามบทบาท — งานหนักใช้โมเดลสูง (orchestrator), งานจัดเก็บใช้ local model (librarian) เพื่อลดต้นทุน — Hermes ตอนนี้เช็กสเปกเครื่องและแนะนำ local model ให้อัตโนมัติ
5. **ความจำ:** เปิด persistent memory ทุกตัว แต่ให้ **ตัวเดียวเขียน external memory (hindsight)** กันข้อมูลขัดแย้งกันเอง
6. **Operations:** terminal backend รันใน Docker เพื่อ isolation, ใช้ workspace ร่วมเป็นที่ส่งไฟล์ถึงกัน, เปิด **keep bots warm** (เพิ่มจาก 3 เป็น 5) + idle timeout ≥10 นาที = ความเร็วต่างกันมาก
7. **3 วิธีสื่อสาร:** ① แชทรายตัว ② bot-to-bot DM (ระวังลูปไม่รู้จบเผาโควตา) ③ **group room** — มีจำกัดจำนวน turns ในตัว กันลูปอนันต์
8. **ผลการทดลอง:** group chat "สีโปรด" ผ่านเร็วมาก ส่วนงานวิจัยจริง (10 แหล่ง / 500 คำ / ต้องมี citation) — orchestrator **ตีงานกลับเพราะไม่มีงานศึกษาปี 2026** แล้ว researcher แก้สำเร็จ (9 แหล่ง) → librarian เสนอโน้ต → อนุมัติ → ไฟล์โผล่ใน Obsidian เชื่อมกราฟความรู้สำเร็จ
9. **Takeaway ตรงๆ:** เอเจนต์เก่งตัวเดียวอาจทำงานนี้ได้ดีเท่า/ดีกว่า — คุณค่าจริงคือปรับแต่งทีมให้งานซ้ำๆ ถูกยกให้ local model ประหยัดต้นทุน และ bot จะ "จำ" ขั้นตอนที่ต้องทำเองหลังให้มัน refine memory (ผู้สร้างประหยัดไป 1 ขั้นการสื่อสาร)

## ใครควรดู
คนที่ใช้ Hermes/agent harness อยู่แล้วและอยากต่อยอดเป็นทีมเอเจนต์ — เน้นแนวคิด "จำกัดสิทธิ์ให้เล็กลงเพื่อความเร็วและประหยัด" มากกว่าโชว์ฟีเจอร์

---
*Attribution: Is Hermes Bot Mode Worth It? — Wanderloots (youtube.com/watch?v=3RoK0rrOHCA), เผยแพร่ 6 ก.ย. 2026*

เสียงพากย์ไทย: ![[3RoK0rrOHCA.mp3]]

