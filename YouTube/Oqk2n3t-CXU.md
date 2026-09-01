---
videoId: "Oqk2n3t-CXU"
title: "First Look at Kimi K3: The Biggest, Smartest Open Weights Model Ever?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=Oqk2n3t-CXU"
published: "2026-07-17"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# First Look at Kimi K3: The Biggest, Smartest Open Weights Model Ever?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=Oqk2n3t-CXU

## 📝 สรุป

# สรุป: First Look at Kimi K3: The Biggest, Smartest Open Weights Model Ever?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~18.5 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Oqk2n3t-CXU

## ประเด็นหลัก

- **Moonshot AI ปล่อย Kimi K3** — โมเดล open weights ระดับ 2.8 ล้านล้านพารามิเตอร์ (2.8T) ถือเป็นโมเดล open ระดับสามล้านล้านพารามิเตอร์ตัวแรกของโลก
- **สเปคเด่น:** context window 1 ล้านโทเคน, สถาปัตยกรรม attention ใหม่ (Kimi Delta Attention + attention residuals + stable lean MoE ที่มี 896 expert แต่ active เพียง 16 ต่อ token)
- **ประสิทธิภาพ scaling** ดีกว่า K2 ประมาณ 2.5 เท่า — คำกล่าวอ้างเรื่อง efficiency สำคัญกว่าขนาดพารามิเตอร์
- **ราคา:** $3 input (cache miss) / $15 output — ใกล้เคียง GPT-5.6 Terra ระดับกลางของ OpenAI ถือว่าแพงแต่เป็น open weights
- **Benchmark:** อยู่ใกล้ด้านบนใน coding/agent benchmark แม้แพ้ Fable และ GPT-5.6 Sol ในบางตัว แต่บางหมวดก็นำ — cost efficiency ดีกว่าคู่แข่งชัดเจน
- **การทดสอบที่ 1 — Front-end coding:** prompt เดิม (One Piece × Star Wars) K3 ทำได้ดีกว่า K2.6 เดิมอย่างชัดเจน — ทรงกลม 3D สมจริงขึ้น, แอนิเมชันครบ, ขัดเกลากว่า
- **การทดสอบที่ 2 — Procedural 3D open world:** สร้างเมืองแฟนตาซี 3D ใน Three.js ได้สวยงาม มีระบบคลิก, texture, แสง ครบ — เทียบได้กับหรือดีกว่าของ Opus 4.8 ในแง่ความครบครัน
- **การทดสอบที่ 3 — Orchestrator + sub-agents:** spawn sub-agent 3 ตัวทำวิจัย paper, สังเคราะห์เป็น top-5 report — มีการ spot-check ความถูกต้องของ paper เอง, ทำงานเสร็จใน <10 นาที, ทำหน้าที่ orchestrator ได้ดี
- **จุดอ่อน:** ยังเป็นรอง Claude 5 และ GPT-5.6 Sol ในภาพรวม, ด้อยกว่าในบาง reasoning/multimodal test — Moonshot เองก็ยอมรับ
- **ข้อจำกัด:** แม้เป็น open weights ก็ไม่สามารถรันบนเครื่องส่วนบุคคลได้ เนื่องจากขนาดใหญ่เกินไป
- **เป้าหมายการออกแบบ:** เน้นงาน long-horizon ที่รันนานเป็นชั่วโมงหรือวัน, รับผิดชอบโปรเจกต์ยากทั้งโปรเจกต์โดยแทบไม่ต้องกำกับ

## ความเห็นสรุป

Kimi K3 เป็นโมเดล open weights ที่สำคัญที่สุดตัวหนึ่งของปี — ไม่ใช่แค่เรื่องขนาด แต่เป็นการผสมผสานระหว่างสถาปัตยกรรม attention แบบใหม่, context window ยักษ์ และการออกแบบเพื่องาน long-horizon แม้จะยังเป็นรองโมเดลปิดท็อปอยู่บ้าง แต่ผลลัพธ์ benchmark และการทดสอบจริงทั้งสามงานแสดงให้เห็นว่ามันเข้าใกล้โมเดลท็อปมากขึ้นเรื่อย ๆ ครับ

เสียงพากย์ไทย: ![[Oqk2n3t-CXU.mp3]]
