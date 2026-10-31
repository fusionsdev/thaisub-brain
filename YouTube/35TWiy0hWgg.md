---
videoId: "35TWiy0hWgg"
title: "Build Databricks AI Agents That Reason & Act | Genie, MCP, Tools"
channel: "Thomas Hass"
url: "https://www.youtube.com/watch?v=35TWiy0hWgg"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-31"
tags: [thai-sub, youtube]
---

# Build Databricks AI Agents That Reason & Act | Genie, MCP, Tools

> [!info] แหล่งที่มา
> Thomas Hass · https://www.youtube.com/watch?v=35TWiy0hWgg

## 📝 สรุป

# สรุป: Build Databricks AI Agents That Reason & Act | Genie, MCP, Tools

- **ช่อง:** Thomas Hass · **ความยาว:** ~27 นาที · **ลิงก์:** https://www.youtube.com/watch?v=35TWiy0hWgg

## ประเด็นหลัก

- ใช้เคส field service technician agent ของบริษัทลิฟต์ ที่ต้องทั้ง troubleshoot จากคู่มือ สร้าง ticket และดูสต็อก/เซ็นเซอร์
- แหล่งข้อมูลสี่ทาง: PDF คู่มือใน SharePoint, Business Central (ERP), Salesforce (CRM/ticket) และ sensor data จากลิฟต์
- นำ ERP/CRM เข้า Databricks (bronze → silver → gold) แล้วสร้าง Genie agent บนตารางที่ join/aggregate แล้ว สำหรับ analytical questions บนข้อมูลประวัติ
- ไม่ควรสร้าง data-access agent แปลง NL→SQL เองเมื่อมีข้อมูลใน Databricks แล้ว — ใช้ Genie ที่ master งานนี้
- Live access ใช้ MCP (Model Context Protocol) ผ่าน AI Gateway เชื่อม Salesforce และ Business Central MCP server แบบกำกับศูนย์กลาง
- ทดสอบใน playground: ถามสต็อกผ่าน Business Central MCP และสร้าง Salesforce case แบบ autonomous ได้จริง
- Sensor realtime แบบ custom ไม่เหมาะกับ MCP ทั่วไป — ใช้ Unity Catalog function (query elevator sensors) กำหนดพารามิเตอร์ unit ID + look back minutes แทน
- Genie = ถามอะไรก็ได้แต่ช้ากว่า / UC function = scope แคบ เร็วกว่า และควบคุมข้อมูลที่ expose ได้
- ชิ้นส่วน (Genie, MCP, tools) ทำงานแยกได้แล้ว ขั้นถัดไปคือ Agent Bricks CLI รวม orchestration พร้อม tracing และ agent memory

## ความเห็นสรุป

คลิปนี้จัดกรอบชัดว่า agent บน Databricks ควรแยก คิดจากข้อมูลประวัติ กับ ลงมือในระบบสด คนละชั้น แล้วเลือก Genie, MCP หรือ Unity Catalog function ตามลักษณะข้อมูล ไม่ยัดทุกอย่างเข้า live API หรือ Genie อย่างเดียว เหมาะเป็นสะพานไปตอน production orchestration ในคลิปถัดไปครับ.

เสียงพากย์ไทย: ![[35TWiy0hWgg.mp3]]

