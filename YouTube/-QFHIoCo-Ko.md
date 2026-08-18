---
videoId: "-QFHIoCo-Ko"
title: "Full Walkthrough: Workflow for AI Coding — Matt Pocock"
channel: "AI Engineer"
url: "https://www.youtube.com/watch?v=-QFHIoCo-Ko"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Full Walkthrough: Workflow for AI Coding — Matt Pocock

> [!info] แหล่งที่มา
> AI Engineer · https://www.youtube.com/watch?v=-QFHIoCo-Ko

## 📝 สรุป

# สรุป: Full Walkthrough: Workflow for AI Coding — Matt Pocock
- **ช่อง:** AI Engineer · **ความยาว:** ~96 นาที · **ลิงก์:** https://www.youtube.com/watch?v=-QFHIoCo-Ko

## ประเด็นหลัก

- **โซนฉลาด vs โซนโง่ (smart zone / dumb zone):** LLM จะทำงานได้ดีที่สุดตอนเริ่มคอนเวอร์เซชันใหม่ ยิ่งใส่ token เข้าไปใน context window มากเท่าไหร่ (ราว 100K ขึ้นไป) มันยิ่งโง่ลงเรื่อยๆ — ต้องแบ่งงานให้เล็กพอที่จะอยู่ในโซนฉลาดเสมอ
- **LLM ลืมเหมือนพระเอก Memento:** แทนที่จะใช้การ compact บทสนทนาให้ยืดเยื้อ ควรล้าง context แล้วเริ่มใหม่ เพื่อให้ทุกเซสชันกลับสู่สภาวะฐานที่เหมือนเดิมเสมอ
- **grill me skill:** ทักษะที่ให้ AI สัมภาษณ์เราอย่างไม่ลดละทีละคำถาม พร้อมคำแนะนำ เพื่อสร้าง "shared understanding" หรือ design concept ร่วมกันก่อนลงมือ — ป้องกันปัญหา misalignment ตั้งแต่ต้น
- **PRD คือเอกสารจุดหมายปลายทาง:** หลังจบ grilling session ให้นำสรุปมาเขียน PRD (product requirements document) แต่ไม่ต้องอ่านมันซ้ำ เพราะ LLM เก่งเรื่องการสรุปอยู่แล้ว จุดสำคัญคือความเข้าใจตรงกัน ไม่ใช่ตัวเอกสาร
- **Kanban board + vertical slices:** แตก PRD เป็นการ์ดงานที่มีความสัมพันธ์แบบ block กัน (ไม่ใช่แผนหลายเฟสแบบเรียงลำดับ) เพื่อให้เอเจนต์หลายตัวทำงานแบบขนานได้ และใช้หลัก traceable bullets — ตัดชิ้นงานแนวตั้งที่ทะลุทุกเลเยอร์ เพื่อให้ได้ feedback เร็ว ไม่ใช่ทำงานทีละเลเยอร์แบบแนวนอน
- **งานสองประเภท:** human in the loop (การวางแผน/การหาความเข้าใจตรงกัน ต้องมีมนุษย์นั่งทำ) vs AFK (implementation ที่ส่งให้เอเจนต์ทำงานห่างจากคีย์บอร์ดได้) — เปรียบเหมือนกะกลางวันกับกะกลางคืน
- **Ralph loop:** พรอมป์ที่ให้เอเจนต์หยิบงานจาก backlog ไป implement ทีละงานแบบ AFK ใน Docker sandbox พร้อม feedback loops (test, type check) — ตัวอย่างสคริปต์ once.sh และโปรเจกต์ Sandcastle สำหรับรันแบบขนาน (planner → implementer → reviewer → merger)
- **TDD (red-green-refactor):** ให้ AI เขียนเทสต์ที่ล้มเหลวก่อนแล้วค่อย implement ทำให้ AI โกงเทสต์ยากขึ้น และเพิ่มคุณภาพของโค้ดเบส
- **feedback loops คือเพดานคุณภาพ:** ถ้าโค้ดเบสไม่มีระบบตรวจสอบที่ดี AI จะเขียนโค้ดแบบมืดบอด — คุณภาพของ feedback loops กำหนดว่า AI เขียนโค้ดได้ดีแค่ไหน
- **deep modules ดีกว่า shallow modules:** โมดูลที่มีอินเทอร์เฟซเล็กแต่ฟังก์ชันภายในเยอะ ทดสอบง่ายและเอเจนต์นำทางได้ — ใช้ skill improve code base architecture หาจุดที่ควรปรับปรุง ออกแบบอินเทอร์เฟซแล้วมอบหมาย implementation (แนวคิด gray box) เพื่อรักษาความเข้าใจโค้ดเบสโดยไม่ต้องรู้ทุกบรรทัด
- **push vs pull:** มาตรฐานการเขียนโค้ดควรเป็นแบบ pull (ให้เอเจนต์ดึงจาก skills เมื่อต้องการ) ในขั้น implementer แต่เป็นแบบ push (ยัดใส่พรอมป์) ในขั้น reviewer อัตโนมัติ
- **QA และ code review ยังเป็นงานของมนุษย์:** อย่าทำให้ทุกขั้นตอนอัตโนมัติจนขาดรสนิยม (slop) — QA คือช่องทางที่มนุษย์ยัดเยียดรสนิยมกลับเข้าสู่โค้ด และสร้าง issues ใหม่กลับเข้าบอร์ดได้ไม่รู้จบ

## ความเห็นสรุป

แมตต์นำเสนอปรัชญาที่ชัดเจนมาก: AI เปลี่ยนวิธีทำงานแต่ไม่ได้ทิ้งหลักวิศวกรรมซอฟต์แวร์ดั้งเดิม — กลับยิ่งต้องยึดหลักเหล่านั้นให้แน่นขึ้น (งานเล็ก ฟีดแบ็กลูปดี โมดูลลึก การทบทวนโค้ด) สิ่งที่โดดเด่นคือการย้ำว่า "โค้ดคือสนามรบ" คุณต้องเข้าใจและควบคุมโค้ดเบสตลอดเวลา ไม่ใช่เมินโค้ดแล้วสั่งสเปกไปเรื่อยๆ แบบ vibe coding และการวางแผนระยะสร้างความเข้าใจตรงกัน (grilling) คือสิ่งที่มนุษย์ต้องทำเองเสมอ ไม่สามารถ delegate ให้ AI ได้

เสียงพากย์ไทย: ![[-QFHIoCo-Ko.mp3]]

