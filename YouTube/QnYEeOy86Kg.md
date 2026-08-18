---
videoId: "QnYEeOy86Kg"
title: "How to Set Up Hermes Agent in Buzz (And Get Agents to Work Together)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=QnYEeOy86Kg"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# How to Set Up Hermes Agent in Buzz (And Get Agents to Work Together)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=QnYEeOy86Kg

## 📝 สรุป

# สรุป: How to Set Up Hermes Agent in Buzz (And Get Agents to Work Together)

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~15 นาที · **ลิงก์:** https://www.youtube.com/watch?v=QnYEeOy86Kg

## ประเด็นหลัก
- วิดีโอสาธิตการตั้งค่า Hermes Agent ใน Buzz (แพลตฟอร์มส่งข้อความสำหรับทีม) ผ่านฟีเจอร์ Gateway โดยแนะนำวิธี native gateway platform ว่าดีที่สุด
- ผู้จัดทำใช้ทีม multi-agent ใน Buzz อยู่แล้ว ทั้งโมเดล Claude, OpenAI และ Hermes Agent บนเครื่องหลายเครื่อง (PC, DJ Spark, VPS)
- ข้อกำหนดเบื้องต้นสำคัญที่สุด: ต้องติดตั้ง Buzz CLI binary ไว้ใน path มิฉะนั้นเอเจนต์จะรับข้อความและรีแอคชันได้ แต่จะไม่มีทางตอบกลับจริง ๆ
- ผู้จัดทำแชร์ repo ชื่อ Dombe Studio / Buzz Skills บน GitHub พร้อม skill 'Hermes and Buzz' ที่ช่วยให้เอเจนต์ติดตั้งและตั้งค่า Buzz CLI ได้เอง
- ขั้นตอนสร้างเอเจนต์ใหม่ (Admiral) จะได้ private key ซึ่งต้องบันทึกไว้เพื่อใช้ตั้งค่า gateway
- การตั้งค่า Hermes Gateway wizard: relay URL คือ community URL, ใส่ Nostr private key, ตั้งค่า allowed users (npub หรือ hex pub keys) เพื่อจำกัดสิทธิ์
- ข้อควรระวัง: ข้อความ error ที่ระบบโชว์อาจไม่ตรงกับสาเหตุจริง เช่น 'agent is not a member of the DM channel' ซึ่งจริง ๆ แล้วปัญหาคือขาด Buzz CLI
- หลังติดตั้ง CLI และรีสตาร์ทเกตเวย์ Admiral ก็ตอบกลับได้ และยังจำหัวข้อสนทนาก่อนหน้าได้ (memory ข้ามแพลตฟอร์ม)
- การสาธิตทำงานร่วมกัน: ให้ Hibana ค้นคว้าอัปเดตล่าสุดของ Buzz แล้วส่งต่อให้ Bulls ตรวจสอบซ้ำ ซึ่ง Bulls ก็ยืนยันทุกจุดพร้อมให้ความเห็น
- ผู้จัดทำมองว่าแนวทางนี้เหมาะกับทีมงาน เพราะเอเจนต์หลายตัวบนเครื่องต่าง ๆ สามารถทำงานร่วมกันใน workspace และ repo เดียวกันได้

## ความเห็นสรุป
วิดีโอให้คำแนะนำแบบ step-by-step ที่นำไปปฏิบัติตามได้จริง ตั้งแต่การเตรียม CLI ไปจนถึงการให้เอเจนต์หลายตัวช่วยกันทำงาน เหมาะสำหรับผู้ที่ใช้ Hermes Agent อยู่แล้วและอยากเชื่อมต่อกับ Buzz หรือต้องการให้เอเจนต์บนเครื่องต่าง ๆ ทำงานร่วมกันเป็นทีม

เสียงพากย์ไทย: ![[QnYEeOy86Kg.mp3]]

