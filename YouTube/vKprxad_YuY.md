---
videoId: "vKprxad_YuY"
title: "Day 5B: Final AI Agent Project — Full End-to-End Build (Complete Course Summary)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=vKprxad_YuY"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 5B: Final AI Agent Project — Full End-to-End Build (Complete Course Summary)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=vKprxad_YuY

## 📝 สรุป

# สรุป: Day 5B: Final AI Agent Project — Full End-to-End Build (Complete Course Summary)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~24 นาที · **ลิงก์:** https://www.youtube.com/watch?v=vKprxad_YuY

## ประเด็นหลัก

- Assignment สุดท้าย (optional) ของคอร์ส: deploy เอเจนต์จากเครื่อง local ขึ้น Vertex AI Agent Engine บน Google Cloud ให้กลายเป็น service พร้อม production
- การสมัคร Google Cloud: ผู้ใช้ใหม่ได้เครดิตฟรี $300 ใช้ได้ 90 วัน ต้องผูกบัตรเครดิตเพื่อยืนยัน (มีการทดสอบหักคืน ~$1) — ไม่ถูกเก็บเงินจนกว่าจะอัปเกรดแพ็กเกจเอง
- การตั้งค่าใน notebook: ลิงก์บัญชีผ่าน Google Cloud SDK (authorization code), ตั้ง project ID จาก Cloud Console (ระวังสับสนกับ project number), ตั้ง GOOGLE_GENAI_USE_VERTEXAI=1 เพื่อใช้ Vertex AI แทน Google AI Studio
- สร้าง weather assistant agent: ใช้โมเดล Gemini 2.5 Flash + tool get_weather (mock ข้อมูลเมือง SF/NY/London/Tokyo/Paris) + instructions แบบเป็นมิตร — สร้างไฟล์ requirements.txt, .env, agent.py ใน agent directory
- Vertex AI Agent Engine: fully managed, autoscaling, มี session management ในตัว, deploy ง่ายด้วย starter pack และมี monthly free tier
- Deployment configuration: min instances = 0 (scale เหลือศูนย์เมื่อไม่ใช้ = ประหยัด), max instances = 1, CPU 1 แกน, memory 1 GiB ต่อ instance — คุมค่าใช้จ่ายต่ำสุด
- เลือก deployment region แบบสุ่มจาก 4 region (Europe West/West 4, US East/Central) — แต่ละคนอาจเห็นต่างกันได้เพราะเป็น random choice
- ขั้น deploy: stage ไฟล์ทั้งหมด → อัปโหลด → containerized deployment (เจอ error ต้อง enable Vertex AI API ครั้งแรก) → ได้ resource name (project/region/reasoning engine/ID)
- ทดสอบด้วย Python SDK: remote agent รับ query "สภาพอากาศ Tokyo" → function call get_weather(city=Tokyo) → function response success + รายงานอากาศ — เห็น stream เบื้องหลังครบ
- Long-term memory ด้วย Vertex AI Memory Bank: session memory ลืมเมื่อจบบทสนทนา (user ต้องบอกซ้ำว่าชอบ Celsius) แต่ memory bank จำถาวรข้าม session — เพิ่ม memory tools + callback/plugin แล้ว deploy ใหม่ ทำงานอัตโนมัติไม่ต้องมี infrastructure เพิ่ม
- Cleanup สำคัญมาก: ลบ deployment ทดสอบเมื่อเสร็จ (force delete remote agent), ปิดเอเจนต์ที่ไม่ใช้, เปิด tracing เพื่อ debug — ไม่งั้นอาจโดนเก็บเงินหลัง 90 วันหรือเกิน $300
- ปิดบัญชีอย่างปลอดภัย: ดู billing ยืนยัน cost = $0 → disable billing → ปิดบัญชี billing (พิมพ์ close) — เปิดใหม่เชื่อมโปรเจกต์กลับได้
- ปิดท้ายด้วยสรุปเส้นทาง 5 วัน (fundamentals → tools → session/memory → observability/evaluation → deployment) และ capstone project (optional) ที่ผู้เข้าร่วมได้ badge + ใบรับรอง Kaggle

## ความเห็นสรุป

วิดีโอนี้เหมาะกับผู้ที่อยากเห็นเส้นทางเต็มจากโค้ดจนถึง production จริงครับ จุดเด่นคือครอบคลุมทั้งเรื่องเทคนิคและการเงิน (free tier, การปิด billing กันโดนเก็บเงิน) ซึ่งมักถูกมองข้ามในคอร์สอื่นครับ ข้อควรระวังคือช่วงท้ายอ้างถึงวันที่และเดดไลน์ใบรับรอง (ธันวาคม 2025 / กุมภาพันธ์ 2026) ซึ่งผูกกับรอบคอร์สของผู้สอน ผู้ดูที่เข้าคอร์สทีหลังควรเช็คเงื่อนไขล่าสุดจากแหล่งทางการเองครับ

เสียงพากย์ไทย: ![[vKprxad_YuY.mp3]]

