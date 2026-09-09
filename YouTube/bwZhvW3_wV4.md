---
videoId: "bwZhvW3_wV4"
title: "Modly: Extensible Open-Source AI 3D Generator"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=bwZhvW3_wV4"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-09-09"
tags: [thai-sub, youtube]
---

# Modly: Extensible Open-Source AI 3D Generator

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=bwZhvW3_wV4

## 📝 สรุป

# สรุป: Modly: Extensible Open-Source AI 3D Generator
- **ช่อง:** DevsKingdom · **ความยาว:** ~9.5 นาที · **ลิงก์:** https://www.youtube.com/watch?v=bwZhvW3_wV4

## ประเด็นหลัก
- Modly โดย Lightning Pixel เป็น เครื่องมือ open-source แปลง รูปภาพ เป็น โมเดล 3D ด้วย AI รัน บน GPU ของ ผู้ใช้
- จุดเด่น คือ ระบบ plugin / extension ให้ เลือก โมเดล ได้ เช่น Hunyuan3D, TripoSG, TRELLIS.2
- รองรับ ทั้ง desktop app (Electron) และ API / SDK สำหรับ automation โดย ไม่ ต้อง พึ่ง UI ตลอด เวลา
- GitHub repo มี ประมาณ 7K stars; readme ครอบคลุม ดาวน์โหลด, virtual environment, และ การ รัน dev
- โครงสร้าง หลัก: โฟลเดอร์ api, extensions, models, และ workspace (เก็บ output เช่น GLB / PLY)
- แต่ละ extension มี dependencies ติดตั้ง ผ่าน pip / setup file; บาง สภาพแวดล้อม เช่น Kaggle ต้อง เขียน requirements เอง
- สตาร์ท เป็น Python REST API ผ่าน uvicorn ที่ พอร์ต 8765 พร้อม endpoint ตาม โมเดล (เช่น create, projection, generate)
- เดโม: generate mesh จาก รูป คน และ รูป รถ ได้ คุณภาพ ดี ภายใน สอง-สาม นาที ด้วย request เดียว
- ใช้ ได้ บน VPS ด้วย curl / POST เพื่อ เรียก API โดย ตรง
- คลิป เน้น ติดตั้ง ฝั่ง API มากกว่า desktop UI

## ความเห็นสรุป
Modly เป็น ตัว เลือก ที่ น่าสนใจ สำหรับ คน ที่ อยาก ได้ image-to-3D แบบ local และ ขยาย โมเดล ด้วย extension. การ มี REST API ทำให้ ต่อ กับ pipeline หรือ agent ได้ ง่าย. เหมาะ กับ ผู้ ที่ คุ้น GPU local และ อยาก ควบคุม โมเดล เอง ครับ.

