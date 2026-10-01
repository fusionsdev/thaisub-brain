---
videoId: "O15SMfGR0lE"
title: "Agent Wikis Beginner's Guide: Building Specialist Agents (local-llm-tinkerer demo)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=O15SMfGR0lE"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-02"
tags: [thai-sub, youtube]
---

# Agent Wikis Beginner's Guide: Building Specialist Agents (local-llm-tinkerer demo)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=O15SMfGR0lE

## 📝 สรุป

# สรุป: Agent Wikis Beginner's Guide: Building Specialist Agents (local-llm-tinkerer demo)
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~23 นาที · **ลิงก์:** https://www.youtube.com/watch?v=O15SMfGR0lE

## ประเด็นหลัก
- specialist agent คือเอเจนต์เฉพาะทางที่รวม skills เครื่องมือ ความรู้ และ guardrails ไว้ในแพ็กเกจเดียวสำหรับหนึ่งงาน ติดตั้งด้วยคำสั่งเดียวบน Hermes Agent
- เหตุผลที่ดีกว่าใช้เอเจนต์ default ตัวเดียว: แยก memories/sessions ไม่ปะปนกับโปรเจกต์อื่น เลือกโมเดลและตั้งค่าให้เหมาะกับงาน และกำหนดขอบเขตการเข้าถึงได้ชัดเจน
- โครงสร้างแพ็กเกจ 6 ส่วน: บุคลิก+house rules (soul.md), expertise (skills คัดแล้ว), knowledge (เข้าถึง agent wikis ผ่าน MCP), tools, routines (cron jobs), และ user guide (guide.md)
- ตัวแรกคือ local LLM tinkerer สำหรับรัน open weight models บนเครื่องตัวเอง: 9 skills 6 wikis 3 tools 3 routines
- หลักปกป้องเครื่อง: โมเดลที่รันเอเจนต์แยกจากโมเดลที่ถูกทดสอบ ห้ามโหลดน้ำหนักโดยไม่ขออนุมัติ ห้ามดาวน์โหลดโดยไม่ถาม รันเซิร์ฟเวอร์ใหญ่ทีละตัว และโค้ดจากโมเดลรันเฉพาะใน sandbox
- tools ที่มาพร้อม: local bench (ทดสอบ latency/concurrency/throughput), memory watchdog (หยุดเฉพาะเซิร์ฟเวอร์ที่ตัวเองดูแล), สูตร quantization EXL2, launch templates สำหรับ vLLM/Docker/llama server
- routines ทั้งสามปิดไว้เริ่มต้น: campaign status (รายงาน 12 บรรทัด), deadline guard (เขียน stop file ครั้งเดียว), nightly regression (เทียบผลกับคืนก่อน)
- เดโมในเทอร์มินัล: ตรวจสิ่งที่ติดตั้งแล้ว สร้าง human eval sandbox รัน local bench campaign บน Qwen 3.8 27B EXL2 จนได้รายงานเต็ม และไล่ดูการเปลี่ยนแปลงของ profile ตามการใช้งาน
- Agent Wikis Pro กำลังเปลี่ยนราคาจาก $9.99 เป็น $19.99/เดือน (1 ตุลาคม) รวม extra large wikis, ~30+ custom skills, exclusive videos, specialist agents และ Q&A newsletter ใน tier เดียว

## ความเห็นสรุป
วิดีโอนี้เหมาะสำหรับคนที่ใช้ Hermes Agent อยู่และอยากจัดระเบียบงานเป็นเอเจนต์เฉพาะทาง แนวคิด "หนึ่งเอเจนต์ต่อหนึ่งงาน" พร้อม guardrails ป้องกันเครื่องพังน่าสนใจมากสำหรับคนเล่น local LLM บนเครื่อง unified memory อย่าง DGX Spark แม้รายละเอียดจะผูกกับ Agent Wikis Pro แต่แนวคิดตั้งค่าเอเจนต์เฉพาะทางนำไปประยุกต์กับ harness อื่นได้เช่นกัน

เสียงพากย์ไทย: ![[O15SMfGR0lE.mp3]]

