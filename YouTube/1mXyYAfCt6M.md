---
videoId: "1mXyYAfCt6M"
title: "Testing Cloudflare OS: Open Source AI Chat + App Builder for the Non-Technical"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=1mXyYAfCt6M"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Testing Cloudflare OS: Open Source AI Chat + App Builder for the Non-Technical

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=1mXyYAfCt6M

## 📝 สรุป

# สรุป: Testing Cloudflare OS: Open Source AI Chat + App Builder for the Non-Technical
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~14 นาที (861 วินาที) · **ลิงก์:** https://www.youtube.com/watch?v=1mXyYAfCt6M

## ประเด็นหลัก
- Cloudflare เปิดโอเพนซอร์ส Cloudflare OS ซึ่งเป็น "ระบบปฏิบัติการเพื่อการทำงานกับ AI" ที่จริงแล้วไม่ใช่ระบบปฏิบัติการ แต่เป็นพื้นที่ทำงานของเอเจนต์ (agent workspace) มากกว่า
- ฟีเจอร์หลักสามอย่าง: agent chat UI (แชตสั่งงานเอเจนต์), การพัฒนาแอปใน sandbox (สร้าง gadgets แล้วแชร์ได้อย่างปลอดภัย), และเฟรมเวิร์กความปลอดภัยชื่อ gatekeepers
- เป้าหมายคือให้คนที่ไม่ใช่สายเทคนิคได้ทดลองสร้างแอปกับ AI ในสภาพแวดล้อมที่ปลอดภัย โดยมี guardrails กำกับทั้งเอเจนต์และ gadgets
- เริ่มต้นใช้งานได้สองวิธี: clone รีโพ Cloudflare/cloudflareos แล้วรันโลคัลด้วย pnpm run local หรือ deploy ผ่าน thisis.os.cloudflare.app/deploy ด้วยบัญชี Cloudflare
- ต้องมี API key เพื่อเชื่อมต่อโมเดล เช่น Claude Sonnet (Anthropic), GPT, Llama, GLM ผ่าน Cloudflare Workers AI
- สร้าง gadget ได้โดยเลือก resource/connection (เช่น GitHub, Google, Supabase, MCP server) แล้วให้เอเจนต์สร้างแอปให้ เช่น แดชบอร์ดค้นหาเอกสาร Cloudflare docs ผ่าน MCP server
- gadgets ที่สร้างเสร็จสามารถเผยแพร่เป็น blueprint (แม่แบบที่แชร์ซ้ำได้) พร้อมลิงก์แชร์ให้ทีม และแชร์ workspace ให้สมาชิกทำงานร่วมกันแบบเรียลไทม์
- เกมโอเอกซ์ (tic-tac-toe) ที่สร้างขึ้นใช้ durable objects และ KV storage ของ Cloudflare เก็บสถานะแบบถาวรโดยไม่ต้องใช้ฐานข้อมูลภายนอก
- ทุกแอปที่สร้างด้วย Cloudflare OS มี agent-friendly API ในตัว ทำให้เอเจนต์ร่วมเล่น/ทำงานกับแอปได้โดยตรง เช่น เล่นเกมกับผู้ใช้
- gatekeepers ทำหน้าที่เป็นชั้นความปลอดภัยเมื่อเชื่อมต่อกับบริการภายนอก: จัดการ authorization, จำลองผลลัพธ์ก่อนการกระทำ และให้มนุษย์อนุมัติ/ปฏิเสธการกระทำที่มีผลข้างเคียง
- โปรเจกต์ยังอยู่ในช่วงต้น (เวอร์ชัน 2) เหมาะกับบริษัท/องค์กรเล็ก ๆ ที่มีทีม มากกว่าเครื่องมือเดี่ยว ๆ สำหรับคนเดียว

## ความเห็นสรุป
Cloudflare OS เป็นเครื่องมือที่น่าสนใจสำหรับผู้ใช้ทั่วไปที่อยากลองสร้างแอปเล็ก ๆ ร่วมกับ AI
ในสภาพแวดล้อมที่ปลอดภัยและแชร์ต่อได้ง่าย โดยเฉพาะผู้ที่อยู่ในระบบนิเวศ Cloudflare อยู่แล้ว
แม้ฟีเจอร์จะยังเรียบง่ายเมื่อเทียบกับโค้ดดิ้งเอเจนต์ระดับมืออาชีพ แต่ก็เป็นจุดเริ่มต้นที่ดี
สำหรับคนที่ไม่ใช่สายเทคนิค และการเป็นโอเพนซอร์สยังเปิดโอกาสให้ปรับแต่งต่อยอดได้อีกมากครับ

เสียงพากย์ไทย: ![[1mXyYAfCt6M.mp3]]

