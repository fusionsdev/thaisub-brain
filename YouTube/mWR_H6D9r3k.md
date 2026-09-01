---
videoId: "mWR_H6D9r3k"
title: "How to Set Up an NVIDIA DGX Spark (And Start Talking to Your Local LLM)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=mWR_H6D9r3k"
published: "2026-07-21"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# How to Set Up an NVIDIA DGX Spark (And Start Talking to Your Local LLM)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=mWR_H6D9r3k

## 📝 สรุป

# สรุป: How to Set Up an NVIDIA DGX Spark (And Start Talking to Your Local LLM)

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~9 นาที · **ลิงก์:** https://www.youtube.com/watch?v=mWR_H6D9r3k

## ประเด็นหลัก

- Tonbi แกะกล่อง NVIDIA DGX Spark เครื่องใหม่ที่ได้รับเป็นของขวัญวันเกิดจากภรรยา เป็นการอัปเกรดจาก RTX 3060 เดิม
- การตั้งค่าเริ่มต้นง่ายมาก เพียงแค่เสียบสายไฟเครื่องก็เปิดขึ้นมาเองโดยอัตโนมัติ
- อุปกรณ์จะสร้าง Wi-Fi hotspot ของตัวเองขึ้นมา ให้เชื่อมต่อจากพีซีโดยใช้รหัสผ่านที่มาพร้อมกับการ์ดในกล่อง
- การเชื่อมต่อที่ง่ายที่สุดคือใช้ NVIDIA Sync ซึ่งจัดการ SSH connection ให้โดยอัตโนมัติ รองรับทั้ง Windows และ Mac OS
- DGX dashboard แสดงข้อมูลระบบครบครัน รวมถึง system memory ที่ 128 GB
- เป็นเครื่องที่ใช้ระบบปฏิบัติการ Linux สามารถติดตั้ง coding agent ต่างๆ ได้ เช่น Hermes Agent, Claude Code, Codex
- ทดลองติดตั้ง Ollama และรันโมเดล Qwen 3.6 27B ได้สำเร็จทันทีหลังตั้งค่า
- โมเดลตอบสนองได้ดี โชว์กระบวนการ thinking ก่อนตอบ แม้จะยังไม่ได้ปรับแต่งอะไรเลย
- ขณะรันโมเดลใช้ memory ประมาณ 42 GB จากทั้งหมด 128 GB
- ผู้จัดวางแผนจะใช้ llama.cpp สำหรับการทดลองและการ tuning local model ในอนาคต
- ผู้จัดแนะนำ agentwikis.com โปรเจกต์ที่ให้บริการ LM wikis ฟรี และมีแบบ pro account เดือนละ $9.99
- ปูทางสำหรับเนื้อหา local model experiments ที่จะตามมาในอนาคตของช่อง

## ความเห็นสรุป

วิดีโอนี้เป็นการแนะนำอุปกรณ์ NVIDIA DGX Spark และโชว์ว่าการตั้งค่านั้นง่ายและตรงไปตรงมามาก แม้แตือุบัติเริ่มต้นก็รวดเร็ว และสามารถรัน local model ได้ภายในเวลาไม่กี่นาทีหลังเปิดกล่อง เป็นจุดเริ่มต้นที่น่าตื่นเต้นสำหรับการทดลอง local model ที่หลากหลายยิ่งขึ้นในอนาคต

เสียงพากย์ไทย: ![[mWR_H6D9r3k.mp3]]
