---
videoId: "8lpG59eugF8"
title: "Day 1B: Agent Architectures — How Modern AI Agents Are Built (Google x Kaggle)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=8lpG59eugF8"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 1B: Agent Architectures — How Modern AI Agents Are Built (Google x Kaggle)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=8lpG59eugF8

## 📝 สรุป

# สรุป: Day 1B: Agent Architectures — How Modern AI Agents Are Built (Google x Kaggle)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~26 นาที · **ลิงก์:** https://www.youtube.com/watch?v=8lpG59eugF8

## ประเด็นหลัก

- ภาค B ของ Day 1 คือการสร้างระบบ multi-agent ตัวแรก ด้วยรูปแบบ LLM as a manager และเรียนรู้ pattern หลัก 3 แบบ: sequential, parallel และ loop
- agent เดี่ยวเมื่อเจองานซับซ้อนจะมี instruction ยืดยาวจนสับสน แก้ยาก ดูแลยาก และไม่น่าเชื่อถือ — ทีม agent เฉพาะทางที่มีหน้าที่ชัดเจนต่างกันสร้างง่าย ทดสอบง่าย และเชื่อถือได้กว่า
- ระบบแรก: research agent (ค้นด้วย Google Search) + summarizer agent (สรุปเป็น bullet 3-5 ข้อ) + coordinator ที่เรียกทั้งสองเป็น tool
- sequential workflow หรือ assembly line: output ของ agent ก่อนหน้าเป็น input ของตัวถัดไป — เหมาะกับ linear pipeline เช่น outline → writer → editor ในการเขียนบล็อก
- parallel workflow: งานอิสระต่อกันรันพร้อมกันเพื่อความเร็ว — ตัวอย่างนักวิจัย 3 หัวข้อ (tech/health/finance) ที่ค้นพร้อมกันแล้วรวมด้วย aggregator เป็น executive briefing
- aggregator ไม่ใช้ Google Search แต่ใช้ output ของ agent ทั้งสามเป็นข้อมูลตั้งต้น
- loop workflow คือ refinement cycle: writer ร่างเรื่องสั้น critic วิจารณ์ แล้ว refiner ตัดสินใจว่าจะเรียก exit loop (เมื่อเจอคำว่า approved) หรือเขียนใหม่ตาม feedback
- loop agent ไม่เข้าใจเองว่า approved คือหยุด จึงต้องสร้าง Python function ชื่อ exit loop และ wrap เป็น function tool ให้ refiner เรียกใช้
- ต้องระบุจำนวน iteration สูงสุดเสมอ (ในตัวอย่างคือ 2) เพื่อกันวงจรวนไม่รู้จบ
- decision tree สรุป: pipeline ตามตัว → sequential, งานขนานอิสระ → parallel, ต้องปรับปรุงคุณภาพวนซ้ำ → loop, ให้ LLM ตัดสินใจเอง → dynamic (LLM orchestrator)
- คอร์สไม่บังคับส่งงาน (no submission required) เรียนตามจังหวะตัวเองได้
- setup ส่วนแรก (install, API key, import ADK, retry) เหมือนภาค A ทุกอย่าง

## ความเห็นสรุป

วิดีโอนี้คือหัวใจของ Day 1 เลยครับ เพราะเปรียบเทียบสถาปัตยกรรม agent ครบทั้งสามแบบพร้อมตัวอย่างโค้ดจริงที่รันได้ตั้งแต่ทีมวิจัยไปจนถึงวงจร writer-critic ครับ คำอธิบาย decision tree ตอนท้ายช่วยให้เลือกใช้ pattern ถูกสถานการณ์ ถือเป็นวิดีโอที่ผู้เรียนควรดูซ้ำและทำ codelab ตามจริงครับ

เสียงพากย์ไทย: ![[8lpG59eugF8.mp3]]

