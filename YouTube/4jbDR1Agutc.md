---
videoId: "4jbDR1Agutc"
title: "Day 2B: Model Context Protocol (MCP) — Full Tutorial & Hands-On Demo"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=4jbDR1Agutc"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 2B: Model Context Protocol (MCP) — Full Tutorial & Hands-On Demo

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=4jbDR1Agutc

## 📝 สรุป

# สรุป: Day 2B: Model Context Protocol (MCP) — Full Tutorial & Hands-On Demo
- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~28 นาที · **ลิงก์:** https://www.youtube.com/watch?v=4jbDR1Agutc

## ประเด็นหลัก
- แบบฝึกหัด Day 2 Part B ของคอร์ส Google × Kaggle 5-Day AI Agents Intensive โฟกัสสอง pattern หลัก คือ MCP integration และ long-running operations
- MCP (Model Context Protocol) คือมาตรฐานเปิดที่ให้ agent ใช้ integration ที่ชุมชนสร้างไว้แล้ว เข้าถึงข้อมูลภายนอกได้โดยไม่ต้องเขียนโค้ดเชื่อมต่อเอง
- ขั้นตอนใช้ MCP มีแค่สี่อย่าง: เลือก MCP server และ tool, สร้าง toolset, เพิ่ม agent เข้ากับการเชื่อมต่อ แล้วรันทดสอบ
- เบื้องหลัง MCP มีการ launch server, handshake สร้างช่องทางสื่อสาร, tool discovery แล้วผลลัพธ์จาก server วนกลับมาที่ agent อย่างราบรื่น
- Demo ใช้ Everything MCP server กับ tool get_tiny_image (ภาพทดสอบ 16x16 pixel แบบ base64) โดยรันผ่าน npx และกรองด้วย tool filter
- Long-running operations / human-in-the-loop คือการให้ tool หยุดค้างรอการอนุมัติจากมนุษย์แล้วจึงทำงานต่อ เช่น ธุรกรรมการเงิน, bulk operations, compliance checkpoint, ค่าใช้จ่ายสูง หรืองานที่ย้อนกลับไม่ได้
- Tool context ให้ความสามารถ request approval และ check approval status เป็นหัวใจของการหยุดรออนุมัติ
- ตัวอย่าง shipping coordinator agent: ออเดอร์ไม่เกิน 5 คอนเทนเนอร์อนุมัติอัตโนมัติ เกิน 5 ให้หยุดรอมนุษย์ตัดสินใจ แล้วคืนสถานะ approved หรือ rejected
- แนวคิดเทคนิคสำคัญ: event (ทุกการเรียก tool/ผลลัพธ์กลายเป็น event), ADK request confirmation event (สัญญาณหยุด) และ invocation ID (key บอก ADK ว่าจะ resume execution ไหน ถ้าไม่มีจะเริ่มใหม่แทน)
- ResumabilityConfig ใช้ห่อ agent เป็น resumable app ที่หยุดแล้วทำต่อได้ ขณะนี้ยังเป็น experimental และอาจเปลี่ยนแปลงในอนาคต
- ทดสอบครบสามสถานการณ์: 3 คอนเทนเนอร์ผ่านอัตโนมัติ, 10 ไป Rotterdam หยุดรอแล้วอนุมัติ, 8 ไป Los Angeles หยุดรอแล้วถูกปฏิเสธ
- แบบฝึกหัด optional: สร้าง agent สร้างภาพผ่าน MCP server ที่ขออนุมัติเมื่อ generate หลายภาพพร้อมกัน

## ความเห็นสรุป
วิดีโอนี้อธิบาย MCP และ human-in-the-loop ได้เป็นระบบดีมาก โดยเดินจากแนวคิดไปสู่โค้ดจริงทีละส่วน จุดเด่นคือการใช้ flowchart ประกอบโค้ด shipping order ทำให้เข้าใจการหยุด-รอ-ทำต่อได้ง่าย และการเน้นว่า invocation ID คือ key ของการ resume ช่วยขจัดความสับสนเรื่อง event handling ซึ่งเป็นส่วนที่ยากที่สุดของแบบฝึกหัดนี้ เหมาะสำหรับคนที่อยากทำ agent ระดับ production ที่ต้องมีการควบคุมและอนุมัติจริงจังครับ

เสียงพากย์ไทย: ![[4jbDR1Agutc.mp3]]

