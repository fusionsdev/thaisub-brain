---
videoId: "79txDFqcrpU"
title: "Adding Vision to a Text-Only LLM: A Local DS4-Flash Experiment"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=79txDFqcrpU"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Adding Vision to a Text-Only LLM: A Local DS4-Flash Experiment

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=79txDFqcrpU

## 📝 สรุป

# สรุป: Adding Vision to a Text-Only LLM: A Local DS4-Flash Experiment

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~22 นาที · **ลิงก์:** https://www.youtube.com/watch?v=79txDFqcrpU

## ประเด็นหลัก
- DeepSeek V4 Flash ที่รันบน DGX Spark เป็นโมเดล text-only ที่เก่งด้านโค้ดและเอเจนต์ แต่ไม่มีวิทัศน์ เพราะเช็กพอยต์ไม่มี vision tower, projector และ image processor
- วิธีแก้แบบเดิมสองแบบไม่น่าพอใจ: เทรนใหม่ให้เห็นภาพ (หนักและใช้เวลาหลายเดือน) หรือสลับไปใช้โมเดล multimodal เล็ก (เสียพลังของ DeepSeek)
- แนวคิดของ Mia AI Lab: 'จ้างตา' ให้โมเดล โดยรันโมเดลวิทัศน์เล็ก (Qwen 3 VL 4B, 4 พันล้านพารามิเตอร์) เป็น sidecar บนพอร์ต 8889 คอยบรรยายภาพเป็นข้อความ แล้วให้ DeepSeek อ่านข้อความนั้นใช้เหตุผลต่อ พิกเซลไม่เคยไปถึงสมอง
- สะพานเชื่อมคือ MCP server ที่มี 3 เครื่องมือ: describe image, OCR image และ compare images (สูงสุด 4 ภาพ) แปลงภาพเป็น base64 แล้วเรียก OpenAI compatible API ของ sidecar
- ตั้งค่า sidecar แบบ deterministic (temperature 0, ปิดการคิด) เพราะมันคือบริการสกัดข้อมูล ไม่ใช่แชตบอต ภาพเดียวกันต้องให้รายงานเดียวกัน
- ราคาที่ต้องจ่าย: KV cache ลดจาก 2.49 ล้านโทเคนเหลือ 1.37 ล้านโทเคน คอนเท็กซ์ลดลง 72% (จาก 240,000 เหลือ 65,000 โทเคน) และต้องปิด memory watchdog ระหว่างเดโม
- ข้อจำกัดคือ 'เกมโทรศัพท์ต่อคำ': ถ้าตาพลาดรายละเอียด สมองก็ไม่มีทางรู้ เพราะฉะนั้นคำอธิบายคือหลักฐาน (evidence) ไม่ใช่ความจริงสูงสุด (ground truth)
- ทดสอบจริง 3 ภาพ: ภาพอนิเมะ 3D cutout (จับได้ว่าตัวละครทำจากกระดาษแข็ง), ภาพ claymation ไดโนเสาร์ (บรรยายละเอียดดี) และ thumbnail ความละเอียดต่ำ (อ่านหัวข้อได้ แต่ hallucinate แผงขวาที่จริงเป็นเพลย์ลิสต์ Spotify)
- ข้อดี: ไม่ต้องเทรนใหม่ ได้พลัง reasoning เต็มของ DeepSeek มีเธรดสนทนาเดียว เปิดปิดได้ และใช้กับแฮร์เนสที่รองรับ MCP ได้ทุกตัว
- ผู้สร้างให้ดาวน์โหลด repo ได้จาก GitHub ของ Mia AI Lab และแนะนำโปรเจกต์ agentwiks.com ของตัวเอง

## ความเห็นสรุป
วิดีโอนี้อธิบายแนวคิด 'เปลี่ยนวิทัศน์ให้เป็นเครื่องมือ' ได้ชัดเจนและทดสอบจริงครบวงจร ทั้งสถาปัตยกรรม การติดตั้ง และข้อแลกเปลี่ยน แม้ระบบจะยังเป็น experimental และมีข้อจำกัดเรื่องคอนเท็กซ์ แต่เป็นแนวทางที่ใช้งานได้จริงกับฮาร์ดแวร์เครื่องเดียว เหมาะสำหรับคนที่รันโมเดล local แล้วอยากได้ความสามารถมองภาพโดยไม่ทิ้งโมเดลหลัก

เสียงพากย์ไทย: ![[79txDFqcrpU.mp3]]

