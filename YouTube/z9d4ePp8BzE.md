---
videoId: "z9d4ePp8BzE"
title: "Exploring Herdr Plugins: Code Review and Git Management"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=z9d4ePp8BzE"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-12"
tags: [thai-sub, youtube]
---

# Exploring Herdr Plugins: Code Review and Git Management

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=z9d4ePp8BzE

## 📝 สรุป

# สรุปภาษาไทย — Exploring Herdr Plugins: Code Review and Git Management

> **ที่มา:** [YouTube — Tonbi's AI Garage](https://www.youtube.com/watch?v=z9d4ePp8BzE) · เผยแพร่ 8 ก.ย. 2026 · ~20:25 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Tonbi's AI Garage*

## วิดีโอนี้เกี่ยวกับอะไร

รีวิว 3 plugins ของ **Herdr** (terminal สำหรับเอเจนต์ที่ผู้สร้างใช้ทุกวัน) ในหมวด code review กับ git management — **Herder reviewer** (รีวิว diff + ให้คอมเมนต์แล้วเอเจนต์แก้ให้) **herder annotate** (คอมเมนต์บนคำตอบของเอเจนต์แล้วส่งกลับเป็น context) และ **Herder file viewer** (ดูไฟล์ markdown แบบ render + เทียบ diff + pin ไฟล์) พร้อมวิธีติดตั้งผ่าน `herder plugin install`

## ประเด็นหลัก

1. **ทำไมต้อง Herdr:** ผู้สร้างลองเครื่องมือเอเจนต์มาเยอะ ตัวที่ติดมือคือ Hermes Agent กับ Herdr — Herdr แทน terminal เดิมทั้งหมด จุดเด่นคือเปิด session ค้างไว้ได้หลายตัว (เช่น บน DGX Spark กับ Windows) ปิดเครื่องแล้วเปิดกลับมาตรงจุดเดิม และรันหลายเอเจนต์พร้อมกัน (Hermes + clawed + codeexes) ให้สั่งงานกันเองได้
2. **Herder reviewer (592 ดาว — ดังสุด):** sidebar รีวิวโค้ดของ Dimmitri Persanov (`persanov/hurder reviewer`) ติดตั้งด้วย `herder plugin install` เปิดด้วย `herder plugin action invoke open plugin` — มีแท็บ Changes / Files / PR (GitHub + GitLab) ใช้เมาส์ได้ไม่ต้องจำคีย์ลัด มี scope ให้เลือกคือ uncommitted / branch / last turn
3. **เวิร์กโฟลว์คอมเมนต์:** สั่งเอเจนต์รีวิว wiki แล้วร่างแผนการตลาด → ไฟล์ใหม่โผล่ใน Changes → กด C คอมเมนต์รายบรรทัด (เช่น double check this / เปลี่ยนแผน 90 วันเป็น 60 วัน) → กด S ส่ง 3 คอมเมนต์ให้เอเจนต์แก้ → ตรวจ diff แล้ว commit ได้เลย แถมสร้าง branch เทียบกับ main ได้
4. **ค้นไฟล์เร็ว:** กด slash command ได้ fuzzy file + live grep (เช่นค้น landing page หรือ strategy) มีพรีวิวไฟล์ให้ดู (ยกเว้นไฟล์รูป)
5. **herder annotate (จาก planotator):** ครึ่งหนึ่งของงานเอเจนต์ไม่ใช่ diff แต่เป็นแผนกับคำตอบ — plugin นี้ให้ annotate ข้อความใน terminal ได้ มีรุ่น full (Mac + Linux) กับ light (ทางเดียวบน Windows) ติดตั้งแล้วเอาบล็อกตั้งค่าใส่ config file (Windows อยู่ใน app data / Linux อยู่ที่ config path) แล้ว reload
6. **วิธีใช้ annotate:** กด prefix (ของเขา Ctrl B) + A บนคำตอบเอเจนต์ → กล่อง annotation เด้งขึ้นมา พิมพ์คอมเมนต์ (เช่น dive deeper on this) กด Ctrl S บันทึก → กด prefix + M จัดการทั้งหมด (ลบ / ล้าง / คัดลอก / archive) → กด prefix + Shift A คัดลอกทุกอันเป็น markdown ส่งกลับเป็น context ให้เอเจนต์ตอบต่อได้เลย
7. **Herder file viewer (523 ดาว — จาก S Marsban):** ทับซ้อน reviewer บ้างแต่เด่นเรื่อง render markdown (ตาราง + headings) ให้อ่านสวย ต้องลง dependencies `glow` `delta` `bat` แล้ว bind ปุ่ม prefix F / prefix Shift F ใน config → ตรวจด้วย `her config check` แล้ว `herder server reload config`
8. **ฟีเจอร์ file viewer:** กด P pin ไฟล์ไว้อ้างอิงขณะเปิดไฟล์อื่น กด V สลับมุมมอง render / diff (ก่อน-หลัง) / plain code มีฟิลเตอร์เฉพาะไฟล์ที่เปลี่ยน กด E เปิดใน editor กด ? ดู help + key bindings
9. **โฆษณาคั่น (claim ของผู้สร้าง ไม่ได้ตรวจสอบอิสระ):** โปรเจกต์ Agent Wikis — wiki มาตรฐานใช้ฟรี ส่วน Pro เดือนละ $9.99 (สมัครตอนนี้ล็อกราคาตลอดชีพ) ที่ agentwiks.com (สะกดตามคำบรรยาย)
10. **ตอนต่อไป:** จะทำวิดีโอ plugins หมวด remote monitoring + approvals (ใช้ herder จากมือถือ) และ orchestration visualization

## ใครควรดู

คนที่ใช้ Herdr (หรือ terminal เอเจนต์ตัวอื่น) ทำงานโค้ดทุกวัน และอยากได้วงจรรีวิวเร็ว — คอมเมนต์บน diff หรือบนคำตอบเอเจนต์แล้วให้มันแก้ให้ทันที แทนการพิมพ์อธิบายซ้ำ

---
*Attribution: Exploring Herdr Plugins: Code Review and Git Management — Tonbi's AI Garage (youtube.com/watch?v=z9d4ePp8BzE), เผยแพร่ 8 ก.ย. 2026*

เสียงพากย์ไทย: ![[z9d4ePp8BzE.mp3]]

