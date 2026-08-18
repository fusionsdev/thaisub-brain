---
videoId: "TfD0sMJGt2M"
title: "Semantica: Open Source Graph-Native Infrastructure for Context"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=TfD0sMJGt2M"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Semantica: Open Source Graph-Native Infrastructure for Context

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=TfD0sMJGt2M

## 📝 สรุป

# สรุป: Semantica: Open Source Graph-Native Infrastructure for Context

- **ช่อง:** DevsKingdom · **ความยาว:** ~14 นาที · **ลิงก์:** https://www.youtube.com/watch?v=TfD0sMJGt2M

## ประเด็นหลัก

- วิดีโอแนะนำโปรเจกต์โอเพนซอร์สชื่อ Semantica ซึ่งเป็น infrastructure แบบ graph-native สำหรับจัดการ context และระบบ AI ที่ตรวจสอบได้ (accountable AI)
- โปรเจกต์แปลง string เป็น context ที่สมบูรณ์แบบกราฟ ช่วยให้ AI agent เข้าใจบริบทและตัดสินใจได้ดีขึ้น ปัจจุบันมีประมาณ 8,000 stars บน GitHub
- readme เปรียบเทียบให้เห็นว่า Semantica ดีกว่าแนวทางดั้งเดิมอย่าง vector DB และ MemGPT รวมถึง plain memory ในการดึงและทำความเข้าใจ context
- สถาปัตยกรรมเริ่มจาก raw context ผ่านการ parse, normalize, แยกเป็น entities และ edges, ตรวจจับความขัดแย้ง (conflict detection), dedupe แล้วสร้าง knowledge graph เก็บใน vector store
- รองรับหลายวิธีในการดึงข้อมูล เช่น graph services, MCP server, CLI และ REST API รวมถึง polyglot graph store สำหรับ export และ visualize
- รองรับ shared context ให้ agent หลายตัวใช้ context ร่วมกันได้ เช่น แชร์ให้ researcher agent, knowledge store หรือทั้งทีม
- เดโมแสดง visualizer ของ Semantica เช่น กราฟข้อมูล Apple Inc. ที่แยกเป็น 114 โหนดและ 11 ขอบ พร้อมฟีเจอร์ temporal scrubber, link prediction, ค้นหา, heatmap, group view และ decision graph
- ฟีเจอร์ decision intelligence ช่วยบันทึก ติดตาม และวิเคราะห์การตัดสินใจ เช่น build graph, record decision, trace decision trend, check decision rules
- เชื่อมต่อกับ coding agents ได้ผ่าน MCP หรือ backend server เช่น Claude Code และ Codex
- ขั้นตอนติดตั้ง: clone repository, pip install, ติดตั้ง openai และ PyCon (สำหรับ vector store กับ embeddings), เริ่ม semantic kernel ผ่าน CLI หรือ REST server และตั้ง environment variables เช่น SEMANTICA_API_KEY_ALLOW_ANONYMOUS (ควรเป็น false ใน production)
- สรุปท้ายวิดีโอแนะนำให้กด subscribe และคอมเมนต์หากมีคำถาม

## ความเห็นสรุป

วิดีโอนี้อธิบาย Semantica ได้ครอบคลุมทั้งแนวคิด สถาปัตยกรรม การใช้งานจริงผ่าน visualizer และขั้นตอนติดตั้งทีละขั้นตอน เหมาะสำหรับนักพัฒนาที่ต้องการให้ AI agent เข้าใจบริบทได้ลึกขึ้นและตรวจสอบการตัดสินใจย้อนหลังได้ครับ อย่างไรก็ตาม คำบรรยายเป็นแบบอัตโนมัติทำให้มีบางคำที่ฟังไม่ชัดหรือเพี้ยนไปบ้าง แต่โดยรวมเนื้อหายังเข้าใจได้ชัดเจน

เสียงพากย์ไทย: ![[TfD0sMJGt2M.mp3]]

