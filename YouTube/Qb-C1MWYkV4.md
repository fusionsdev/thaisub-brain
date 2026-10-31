---
videoId: "Qb-C1MWYkV4"
title: "FREE 32GB VRAM Server for Running AI Models Locally"
channel: "Abi"
url: "https://www.youtube.com/watch?v=Qb-C1MWYkV4"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-31"
tags: [thai-sub, youtube]
---

# FREE 32GB VRAM Server for Running AI Models Locally

> [!info] แหล่งที่มา
> Abi · https://www.youtube.com/watch?v=Qb-C1MWYkV4

## 📝 สรุป

# สรุป: FREE 32GB VRAM Server for Running AI Models Locally

- **ช่อง:** Abi · **ความยาว:** ~9 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Qb-C1MWYkV4

## ประเด็นหลัก

- ใช้ GPU ฟรีบน Kaggle เพื่อรันโมเดล AI ขนาดใหญ่ โดยไม่ต้องมี GPU แรงในเครื่องตัวเอง
- สร้าง Kaggle notebook แล้วเปิด acceleration เป็น GPU T4 x2 (Nvidia T4 สองตัว รวม VRAM ประมาณ 32 GB)
- ติดตั้งและสตาร์ท Ollama บน notebook เพื่อดาวน์โหลดและรันโมเดล
- เลือกโมเดลจาก Hugging Face ในรูปแบบ GGUF ที่เข้ากับ Ollama เช่น quantized Q4_K_M
- ใช้ Cloudflare tunnel สร้าง public HTTPS URL ชั่วคราว ชี้ไปที่ Ollama server บน Kaggle
- บนเครื่อง local ตั้ง custom endpoint แบบ OpenAI compatible โดยเติม `/v1` ท้าย tunnel URL
- ถ้า client ถาม API key ใส่ placeholder เช่น Ollama ได้ แต่ไม่ใช่ระบบความปลอดภัยจริง
- ทดสอบผ่าน coding agent ใน terminal ด้วย prompt ง่ายๆ เพื่อยืนยันว่า request ไปประมวลผลบน Kaggle
- ชื่อที่โมเดลรายงานเองไม่น่าเชื่อถือเสมอ ควรดูชื่อจาก client config หรือ API
- Kaggle มีโควตา GPU และจำกัด session เหมาะเรียน/ทดลอง มากกว่า production ต่อเนื่อง

## ความเห็นสรุป

คลิปสั้น ชัด เป็น walkthrough ติดตั้งจริงตั้งแต่ notebook ถึง terminal บนเครื่อง local.
จุดแข็งคือรวม Ollama + Hugging Face + Cloudflare tunnel เป็น pipeline เดียวที่ทำตามได้.
ข้อจำกัดสำคัญคือ tunnel ชั่วคราวและความเสี่ยง URL สาธารณะ รวมถึงโควตา Kaggle ที่ไม่เหมาะงาน production ยาวๆ.

เสียงพากย์ไทย: ![[Qb-C1MWYkV4.mp3]]

