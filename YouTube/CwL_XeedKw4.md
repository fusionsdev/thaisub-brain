---
videoId: "CwL_XeedKw4"
title: "I Gave Claude a Second Brain (It Remembers Everything)"
channel: "Leon van Zyl"
url: "https://www.youtube.com/watch?v=CwL_XeedKw4"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-02"
tags: [thai-sub, youtube]
---

# I Gave Claude a Second Brain (It Remembers Everything)

> [!info] แหล่งที่มา
> Leon van Zyl · https://www.youtube.com/watch?v=CwL_XeedKw4

## 📝 สรุป

# สรุป: I Gave Claude a Second Brain (It Remembers Everything)
- **ช่อง:** Leon van Zyl · **ความยาว:** ~10.7 นาที · **ลิงก์:** https://www.youtube.com/watch?v=CwL_XeedKw4

## ประเด็นหลัก
- ปัญหา: จำได้ว่าเคยเห็นข้อมูลจากวิดีโอไหน แต่นึกไม่ออกว่าวิดีโอไหน — อยากให้ AI ค้นและอ้างแหล่งเดิมให้
- โซลูชัน: Progress Agentic RAG — ใช้ได้กับ Claude, ChatGPT, Hermes Agent
- เหตุผลที่ไม่ใช้ไฟล์ Markdown: ขยายตัวไม่ได้ ช้า ไม่เหมาะกับ agent; RAG + vector database เร็วกว่ามาก
- สถาปัตยกรรม: Cowork เพิ่มไฟล์ → Progress เปลี่ยนไฟล์เป็นฐานข้อมูลค้นได้ → Claude แชทค้นเมื่อถาม
- เริ่มต้น: สมัครที่ rag.progress.cloud → สร้าง knowledge box (เลือก region, embedding model, GDPR anonymization ได้)
- อัปโหลด: ใช้ agent ที่รันสคริปต์ได้ (Cowork / ChatGPT work mode / Hermes Agent) + พรอมต์ให้สร้าง uploader ที่ใช้ซ้ำได้ (ตั้งค่าครั้งเดียว)
- ต้องใช้ NucliaDB API endpoint + API key (role: manager) — แนะนำให้ agent ตั้งค่าก่อนแล้วใส่ key ทีหลัง
- เดโม: อัปโหลด NASA ScienceCasts 15 วิดีโอจาก archive.org (รวม Dark Lightning) — ค้นแล้วได้ทั้งคำตอบและแหล่งที่มา
- การค้น: ต่อ MCP server endpoint ผ่าน connectors (add → ตั้งชื่อ → วาง URL → OAuth register automatically) ได้เครื่องมือ batch get documents / get document / search documents
- ใช้ได้ทั้ง Claude Desktop และ claude.ai — sync อัตโนมัติ ใช้ได้ทุกที่
- สปอนเซอร์: Progress

## ความเห็นสรุป
บทสอนที่ละเอียดตั้งแต่สมัครจนใช้งานจริง เหมาะกับมือใหม่เพราะทำตามทีละคลิกได้เลย แนวคิด "สมองที่สองแบบ RAG" แก้จุดอ่อนของการเก็บ Markdown ได้จริง และการให้ agent ดูแลการอัปโหลดเองทำให้ระบบอยู่ตัวในระยะยาวครับ

เสียงพากย์ไทย: ![[CwL_XeedKw4.mp3]]

