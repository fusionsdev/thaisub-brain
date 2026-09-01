---
videoId: "tVED0r3vGrQ"
title: "I Put an Agent Skill on the Solana Blockchain (Real Code Bytes)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=tVED0r3vGrQ"
published: "2026-07-13"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# I Put an Agent Skill on the Solana Blockchain (Real Code Bytes)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=tVED0r3vGrQ

## 📝 สรุป

# สรุป: I Put an Agent Skill on the Solana Blockchain (Real Code Bytes)
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~21 นาที · **ลิงก์:** https://www.youtube.com/watch?v=tVED0r3vGrQ

## ประเด็นหลัก
- ผู้สร้างสร้างโปรเจกต์ "Gitlana" เพื่อจัดเก็บ agent skill (โค้ดจริง) ไว้บน Solana blockchain แบบถาวร ไม่ใช่ลิงก์หรือไฟล์สำรอง แต่เป็น bytes จริงใน account เดียว
- แนวคิดเริ่มจากคำถาน่าสนใจ "ถ้า repo สามารถเป็น NFT ได้ล่ะ?" และพัฒนาเป็นบ้านถาวรที่ตรวจสอบได้สำหรับแพ็กเกจซอฟต์แวร์ขนาดเล็ก
- เหตุผลหลักในการทำ: (1) พื้นที่เก็บข้อมูลที่ไม่มีใครแตะต้องได้ (2) มี wallet ติดกับทุกแพ็กเกจเป็น identity (3) "คิดว่ามันเท่"
- ใช้ Metaplex Core standard โดยเก็บ manifest ไว้ใน attributes plugin และตัวโค้ดเองใน app data plugin
- แพ็กเกจตัวอย่างมีขนาด 3,297 bytes บน mainnet ใช้เวลาสร้างด้วย Claude Code + Fable และ Hermes agent (GPT-5.6 Sol)
- deterministic packaging ทำให้ source เดียวกันได้ archive ตรงกันทุก byte บนทุกเครื่อง ใครก็ rebuild แล้วยืนยัน fingerprint ได้
- การ publish บน mainnet เสียค่าใช้จ่ายประมาณ 0.05 SOL (~$4) และเป็นเงินมัดจำที่คืนได้ ทั้งยังมี proposal จะลดอีก 10 เท่า
- รองรับ versioning เหมือน GitHub: update แทนที่ในตำแหน่งเดิม (เสียค่าใช้จ่ายน้อย) และ release เป็น snapshot แยกที่ immutable
- การเข้าถึงฟรีทั้งหมด เพียงเรียก get account info ไม่ต้อง login ตรวจสอบ fingerprint แล้วก็ unpack + ติดตั้งได้
- เดโมจริง: ให้ Hermes agent ตัวใหม่เอี่ยมดึงและติดตั้ง skill จาก address เดียว สำเร็จในราว 4 นาที
- Road map: Phase 2 เป็น provenance (เชื่อม wallet กับผู้เขียนตั้งต้นด้วย NPM provenance tech), Phase 3 คือ machine payments (Tempos / X402)
- โค้ดทั้งหมดเป็น public บน GitHub (Tomb Studios/Gitlana) และมี CLI ให้ใช้สำหรับ mint package ได้

## ความเห็นสรุป
โปรเจกต์นี้เป็นการทดลองที่น่าสนใจและมีเทคนิคที่ค่อนข้างแข็งแรง โดยอาศัยความสามารถของ Metaplex Core app data plugin ในการเก็บ raw bytes บน chain แบบถาวรจริงๆ แม้ว่าข้อจำกัดเรื่องขนาดและต้นทุนยังทำให้ใช้ได้กับแพ็กเกจขนาดเล็กเท่านั้น แต่แนวคิดดังกล่าวเปิดทางใหม่ในการกระจายซอฟต์แวร์อย่างไม่มีศูนย์กลาง คุ้มค่ากับการติดตามต่อสำหรับทิศทาง phase 2 และ 3 ครับ

เสียงพากย์ไทย: ![[tVED0r3vGrQ.mp3]]
