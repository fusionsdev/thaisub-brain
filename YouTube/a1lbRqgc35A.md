---
videoId: "a1lbRqgc35A"
title: "Complete AI Agent Project in Gemini — Multi-Agent Tools, Memory & Deployment (Capstone)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=a1lbRqgc35A"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Complete AI Agent Project in Gemini — Multi-Agent Tools, Memory & Deployment (Capstone)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=a1lbRqgc35A

## 📝 สรุป

# สรุป: Complete AI Agent Project in Gemini — Multi-Agent Tools, Memory & Deployment (Capstone)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~19 นาที · **ลิงก์:** https://www.youtube.com/watch?v=a1lbRqgc35A

## ประเด็นหลัก

- ตอนปิดซีรีส์: จบ assignment ทั้ง 10 อันแล้ว เหลือ capstone project (optional) — เข้าร่วมแล้วได้ badge + ใบรับรองบนโปรไฟล์ Kaggle และถ้าติด top 12 ได้ swag + โชว์ผลงานบนโซเชียลมีเดียของ Kaggle
- 4 track ให้เลือก: concierge agent, agents for good, enterprise agents, freestyle — ผู้สอนเลือก concierge agent
- เงื่อนไขหลัก: write-up ที่มี problem + solution pitch, เผยแพร่โค้ดแบบ public (GitHub หรือ Kaggle notebooks), อธิบายคุณค่าของเอเจนต์ให้ได้ และส่งได้ครั้งเดียวต่อโปรเจกต์ (retract ได้แต่ทำซ้ำไม่ได้)
- Bonus 10 คะแนน: อัดวิดีโอ demo (หน้าจอการทำงาน) ใส่ลิงก์ YouTube ใน write-up
- Write-up ต้องมี checklist 6 ข้อ: title, subtitle (optional), thumbnail, track, description (markdown ≤ 1500 คำ ครอบคลุม problem statement, เหตุผลที่เลือก track, architecture, tools, demo), project link
- โปรเจกต์ของผู้สอน: AI learning planner แบบ concierge — แก้ปัญหาแหล่งเรียนรู้กระจัดกระจาย ไม่มีเส้นทางเรียนแบบมีระบบ และรักษาความสม่ำเสมอยากเมื่อเวลาจำกัด
- สถาปัตยกรรม: coach agent (หน้าบ้าน สนทนากับผู้ใช้) มอบหมายงานให้ planner agent ผ่าน agent tool calling; tools คือ search_resources + build_schedule (วางแผน 3/5/7 วันตามชั่วโมงต่อสัปดาห์)
- เทคโนโลยี: Gemini 2.5 Flash ผ่าน Google GenAI API, Google ADK, InMemory session service, Kaggle notebook, observability + evaluation harness ตรวจโครงสร้างแผน (จำนวนวัน/ชั่วโมง) และ error handling
- Demo จริง: "อยากเรียน AI สำหรับ YouTube, beginner, 5 ชม/สัปดาห์" → ได้แผน 5 วันแบบ personalized พร้อมคำอธิบายฉบับเป็นมิตร; evaluation ผ่านทั้งเคส 3 ชม./สัปดาห์ และ 8 ชม./สัปดาห์
- การจัดการ rate limit ของ free tier API: ป้องกัน notebook พัง ทำงานต่อเนื่องแบบ graceful พร้อมข้อความสถานะที่เป็นมิตร
- เทคนิคจัดการรูปใน Kaggle: สร้าง dataset ใหม่ อัปโหลดรูป แล้ว add input เข้า notebook อ้างอิง image ID ในโค้ด — แชร์แบบ public เพื่อให้กรรมการเข้าถึงได้

## ความเห็นสรุป

วิดีโอนี้เหมาะเป็นแบบอย่างสำหรับคนที่อยากส่ง capstone จริง เพราะเห็นทั้งกติกา โครงสร้าง write-up และโค้ดจริงของผู้สอนครบตั้งแต่ต้นจนจบครับ โปรเจกต์ AI learning planner เป็นตัวอย่างที่เหมาะสม เพราะรีใช้ทุกอย่างที่เรียนมาในคอร์ส (multi-agent, tools, session, evaluation, observability) ไว้ในงานเดียวครับ ข้อควรจำคือ deadline และเงื่อนไขรางวัลผูกกับรอบ hackathon ของผู้สอน ผู้ดูควรเช็คข้อมูลล่าสุดจากหน้ากากับ Kaggle เองครับ

เสียงพากย์ไทย: ![[a1lbRqgc35A.mp3]]

