---
videoId: "cPKwycZ_FtY"
title: "Trying Out Matt Pocock's NEW /wayfinder Skill in Hermes Agent"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=cPKwycZ_FtY"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Trying Out Matt Pocock's NEW /wayfinder Skill in Hermes Agent

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=cPKwycZ_FtY

## 📝 สรุป

# สรุป: Trying Out Matt Pocock's NEW /wayfinder Skill in Hermes Agent

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~30 นาที · **ลิงก์:** https://www.youtube.com/watch?v=cPKwycZ_FtY

## ประเด็นหลัก

- ผู้สร้างวิดีโอทดลองใช้สกิล Wayfinder ตัวใหม่ของ Matt Pocock ใน Hermes Agent เป็นครั้งแรก โดย Wayfinder เป็นเวอร์ชันขั้นสูงของ Grill Me ที่ออกแบบมาสำหรับโปรเจกต์ขนาดใหญ่
- Wayfinder แบ่งงานออกเป็นหลายเซสชัน ใช้ decision tickets (ตั๋วการตัดสินใจ) และมีตั๋วหลายประเภท ได้แก่ research, prototyping, grilling, tasking, fog of war และ scope
- โจทย์ทดสอบคือการวางแผนสร้างเกม puzzle platformer ชื่อชั่วคราวว่า Token Burn ซึ่งมีเอเจนต์เป็นตัวละครคู่หูที่ผู้เล่นสั่งงานได้ โดยเอเจนต์ใช้ tokens เป็นเชื้อเพลิงจำกัดต่อด่าน
- เริ่มต้นด้วยโมเดล GPT 5.6 Terra ในแอปเดสก์ท็อปของ Hermes Agent เพราะงานนี้เน้นการวิจัยและวางแผนมากกว่าการเขียนโค้ด
- Wayfinder ถามคำถามชุดแรกเพื่อกำหนดจุดหมาย ผลลัพธ์คือ production-ready vertical slice specification และ implementation roadmap โดยไม่ต้องสร้างเกมจริงในขั้นวางแผน
- ระบบสร้างแผนที่การตัดสินใจ (map) และตั๋วย่อย 6 ใบ ใช้ตัวสำรอง tracker แบบ markdown ในเครื่องใต้โฟลเดอร์ .wayfinder (ไม่จำเป็นต้องใช้ GitHub)
- เปิด research ticket แบบ AFK สองใบรันพร้อมกัน แล้วให้เอเจนต์สร้างเซสชันแยกเพื่อทำงานตั๋ว grilling ที่เหลือ รวมถึงเซสชันที่ถามคำถามถึง 64 ข้อ
- แต่ละตั๋วเมื่อเสร็จจะบันทึกการตัดสินใจ เหตุผล acceptance constraints และลิงก์อ้างอิงในไฟล์ markdown แล้วปิดตั๋ว พร้อมอัปเดตแผนที่กลาง
- ได้ prototype การวางแผนสำหรับ tutorial-to-capstone stage progression ออกมาเป็นไฟล์ markdown พร้อมไดอะแกรม ผู้สร้างตรวจทานและยืนยัน
- ขั้นสุดท้าย Wayfinder สร้างไฟล์ส่งต่องาน (implementation handoff) ขนาดใหญ่ พร้อมคำแนะนำสำหรับ Hermes ให้ใช้ sub-agent driven development เพื่อลงมือสร้างเกมจริง
- ความเห็นส่วนตัว: ประทับใจโครงสร้างของ Wayfinder โดยเฉพาะการแยกหัวข้อเป็นเซสชันๆ การส่ง sub-agents ไปวิจัย และแนวคิด fog of war ว่าจะตั้งตั๋วได้เมื่อคำถามชัดเจนแล้วเท่านั้น
- อนาคต: จะลงมือสร้างเกมจริงด้วย Grok 4.5/4.6 ใน Grok Build หรือ Hermes Agent ในวิดีโอถัดไป และโปรโมตโปรเจกต์ agentwikis.com (วิกิฟรี พร้อมบัญชี pro $9.99/เดือน)

## ความเห็นสรุป

วิดีโอนี้เป็นบททดลองใช้ Wayfinder แบบสดๆ ครั้งแรกที่เห็นภาพชัดเจนว่าสกิลวางแผนระดับโปรเจกต์ทำงานอย่างไร ตั้งแต่การตั้งจุดหมาย การสร้างแผนที่การตัดสินใจ การกระจายงานเป็นตั๋วไปยังหลายเซสชัน ไปจนถึงการส่งมอบเอกสาร implementation ที่พร้อมให้เอเจนต์เขียนโค้ดลงมือทำต่อได้ทันที เหมาะสำหรับผู้ที่สนใจการทำงานกับ AI agents และการวางแผนโปรเจกต์ซอฟต์แวร์ขนาดใหญ่ครับ

เสียงพากย์ไทย: ![[cPKwycZ_FtY.mp3]]

