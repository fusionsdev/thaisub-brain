---
videoId: "lMq6FDhFHrA"
title: "MiniMax H3 + WanGP + ComfyUI: Seedance 2.5 Open Source Low VRAM Competitor Complete Easy Setup Guide"
channel: "DevsKingdom"
url: "https://www.youtube.com/watch?v=lMq6FDhFHrA"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# MiniMax H3 + WanGP + ComfyUI: Seedance 2.5 Open Source Low VRAM Competitor Complete Easy Setup Guide

> [!info] แหล่งที่มา
> DevsKingdom · https://www.youtube.com/watch?v=lMq6FDhFHrA

## 📝 สรุป

# สรุป: MiniMax H3 + WanGP + ComfyUI: Seedance 2.5 Open Source Low VRAM Competitor Complete Easy Setup Guide

- **ช่อง:** DevsKingdom · **ความยาว:** ~8 นาที · **ลิงก์:** https://www.youtube.com/watch?v=lMq6FDhFHrA

## ประเด็นหลัก

- MiniMax H3 เป็นโมเดลวิดีโอ AI แบบโอเพนซอร์สที่เพิ่งเปิดตัว ประมาณหนึ่งถึงสองสัปดาห์ก่อนหน้านี้ มีคุณภาพสูง เทียบชั้นได้กับ Sora 2.0 และ Sora 2.5
- ทาง ComfyUI ก็ปล่อยเวิร์กโฟลว์พร้อมตัวอย่างวิดีโอจำนวนมาก แต่ทุกแพลตฟอร์มยังต้องดาวน์โหลดโมเดลซึ่งมีขนาดใหญ่มาก แม้แต่เวอร์ชัน compact (FP8) หรือเวอร์ชัน pruned ก็ยังใหญ่
- การทดลองใช้บนเครื่องสเปกต่ำทำได้ยากเพราะต้องใช้ฮาร์ดแวร์และ VRAM เยอะ วิธีแก้คือใช้ Kaggle ซึ่งรองรับ VRAM ต่ำกว่า 16 กิกะไบต์ได้ฟรี
- เครื่องมือหลักคือ WanGP เฟรมเวิร์กสำหรับ GPU ความจำต่ำ ใช้สร้างวิดีโอ MiniMax H3 บน GPU ระดับล่างได้ผลลัพธ์ดี ใช้งานผ่านทั้งเว็บ UI และ SDK
- บน UI ตั้งค่าได้หลากหลาย เช่น LoRA (รวมถึง first-step LoRA) โมเดล 33B และ pruned 20B การเพิ่มโมเดลของตัวเอง (checkpoint, text encoder, VAE) ด้วยการดาวน์โหลดจาก Hugging Face แล้วระบุพาธในโฟลเดอร์ temp ของ Kaggle
- ตั้งค่าขนาด (เช่น 480) จำนวนเฟรม (5 หรือ 10 วินาที) และ inference steps ซึ่งค่าเริ่มต้นคือ 4 เพราะใช้ turbo LoRA จากนั้นกด generate ได้เลย
- ขั้นตอนติดตั้งใน Kaggle notebooks: ดาวน์โหลด WanGP ลงโฟลเดอร์หลัก ลง dependencies ดาวน์โหลดโมเดลสามตัวลง temp/minimax H3 แล้วเปิดใช้งาน
- ต้องใช้ Cloudflare tunnel (port 7860 ชี้ไป localhost) เพราะ Gradio หรือ ngrok ช้าเกินไปสำหรับการใช้งานผ่านเทอร์มินัล
- การใช้ SDK: ระบุโฟลเดอร์ WanGP ตั้งค่าพารามิเตอร์และ exporter settings ซึ่งสำคัญมากสำหรับกำหนดโมเดล จากนั้นส่งงาน (submit task) และดาวน์โหลดวิดีโอจากโฟลเดอร์ output

## ความเห็นสรุป

วิดีโอนี้เป็นคู่มือลงมือทำจริงที่ครบถ้วนสำหรับคนที่อยากลองโมเดลวิดีโอโอเพนซอร์สบนฮาร์ดแวร์จำกัด โดยไม่ต้องเสียเงินซื้อ GPU แรงๆ แม้คำบรรยายจะเป็นแบบอัตโนมัติและมีชื่อบางชื่อเพี้ยนไปบ้าง แต่เนื้อหาหลักคือแนวทางติดตั้งและใช้งาน WanGP บน Kaggle ยังเข้าใจได้ชัดเจน เหมาะสำหรับผู้ที่พอมีพื้นฐานการใช้ Kaggle และ ComfyUI อยู่บ้าง

เสียงพากย์ไทย: ![[lMq6FDhFHrA.mp3]]

