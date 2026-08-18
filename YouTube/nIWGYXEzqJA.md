---
videoId: "nIWGYXEzqJA"
title: "Oracle Fusion AI Studio - The Complete Enterprise Coding Agent Workflow"
channel: "Leon van Zyl"
url: "https://www.youtube.com/watch?v=nIWGYXEzqJA"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Oracle Fusion AI Studio - The Complete Enterprise Coding Agent Workflow

> [!info] แหล่งที่มา
> Leon van Zyl · https://www.youtube.com/watch?v=nIWGYXEzqJA

## 📝 สรุป

# สรุป: Oracle Fusion AI Studio - The Complete Enterprise Coding Agent Workflow
- **ช่อง:** Leon van Zyl · **ความยาว:** ~22 นาที · **ลิงก์:** https://www.youtube.com/watch?v=nIWGYXEzqJA

## ประเด็นหลัก
- Oracle ใช้ coding agents (เอเจนต์ AI ช่วยเขียนโค้ด) สร้างและขยาย Oracle Fusion Applications ซึ่งเป็นระบบหลังบ้านของบริษัทใหญ่กว่า 14,000 แห่งทั่วโลก ครอบคลุม HR, การเงิน, จัดซื้อจัดจ้าง, ซัพพลายเชน, การขาย และการตลาด
- ลูกค้ากว่า 7,000 รายใช้ฟีเจอร์ Fusion AI อยู่แล้ว ซึ่งช่วยให้สร้างส่วนขยาย (extensions) บนแอปพลิเคชันด้วย AI agent ได้ โดยถ่ายทอดความรู้เฉพาะทางลงใน agent skills พร้อมตัวอย่าง prompt ที่ใช้กับ Codex หรือ Claude Code ได้
- ขั้นตอนทั้งหมด: ผู้ใช้แชตกับ coding agent บนเครื่องตัวเอง → agent ใช้ AI Studio skill และ CLI tool เชื่อมต่อไปยัง Fusion Studio บนคลาวด์เพื่อดึง pattern เดิม → สร้างไฟล์ (app file, workflow files) → ส่งไปตรวจสอบที่ Fusion Cloud → ผ่านแล้วจึงสร้างหน้าจอและเผยแพร่ให้ผู้ใช้
- กฎข้อที่ 1: spec ต้องมาก่อน (the spec comes first) — จะไม่สร้างอะไรจนกว่าจะมีแผนและทุกฝ่ายตกลงกัน
- กฎข้อที่ 2: ทุกอย่างเป็น read only ตามค่าเริ่มต้น จนกว่าจะสั่งให้เพิ่มความสามารถในการสร้าง/แก้ไขข้อมูลอย่างชัดเจน
- กฎข้อที่ 3: discover before you build — agent ต้องสำรวจโค้ด/pattern/workflow ที่มีอยู่ก่อนเสมอ ก่อนสร้างของใหม่จากศูนย์
- กฎข้อที่ 4: structure over improvisation — agent ต้องทำตามกฎและ guardrails ที่กำหนดใน skill files ไม่สามารถมั่วหรือทำตามอำเภอใจ
- กฎข้อที่ 5: unvalidated means unfinished — งานจะถือว่าเสร็จก็ต่อเมื่อผ่านการตรวจสอบ (validation) ในระบบแล้วเท่านั้น
- การติดตั้งตั้งค่าง่ายมาก: ดาวน์โหลด agent skills จาก public repo, ติดตั้ง VS Code extension, ตั้งค่า authentication ผ่าน Fusion AI Studio แล้วคัดลอกสกิลลงโฟลเดอร์ .agents/skills ก็ใช้งานได้ โดยไม่จำเป็นต้องเป็นนักพัฒนา
- Demo จริง: สร้างแอป succession planning ผ่าน prompt ภาษาเดียวกับผู้ใช้ทั่วไป → agent ทำ discovery, เสนอ spec/MVP, สร้างแอป 2 ตัวโดยไม่มี error, deploy แบบ draft ไปยัง Fusion Cloud และทำงานกับข้อมูลสดจริง (เช่น ระบุว่า Sophie Bromley มีความเสี่ยงสูงและแนะนำผู้สืบทอดคือ Emily และ Olivia ผ่าน Ask Oracle)
- แพลตฟอร์มแบบนี้เข้าถึงยาก (มักต้องเป็นพาร์ทเนอร์ของ Oracle) วิดีโอจึงมีจุดประสงค์เพื่อการศึกษา และสอนแนวคิดที่นำไปใช้กับแอปของตัวเองหรือทีมพัฒนาขนาดใหญ่ได้

## ความเห็นสรุป
วิดีโอนี้เป็นกรณีศึกษาที่ดีมากสำหรับการออกแบบ coding agent ระดับองค์กร โดยเฉพาะแนวคิด "spec มาก่อน", "สำรวจก่อนสร้าง" และ "ยังไม่ผ่านการตรวจสอบ = ยังไม่เสร็จ" ที่ช่วยลดความเสี่ยงและทำให้ agent ทำงานอยู่ในกรอบที่ควบคุมได้ จุดที่โดดเด่นที่สุดคือการถ่ายทอดความรู้ของผู้เชี่ยวชาญลงใน agent skills ที่ใครก็ใช้ตามได้ ซึ่งเป็นแม่แบบ (blueprint) ที่ทีมพัฒนาองค์กรอื่นนำไปลอกเลียนแบบได้จริง

*สรุปนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

เสียงพากย์ไทย: ![[nIWGYXEzqJA.mp3]]

