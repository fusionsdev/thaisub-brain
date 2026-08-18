---
videoId: "Eq0vyEZZXJc"
title: "Pushing Qwen3.8-27B to the Limit: How a Small Local LLM Handles Challenging Tasks"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=Eq0vyEZZXJc"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Pushing Qwen3.8-27B to the Limit: How a Small Local LLM Handles Challenging Tasks

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=Eq0vyEZZXJc

## 📝 สรุป

# สรุป: Pushing Qwen3.8-27B to the Limit: How a Small Local LLM Handles Challenging Tasks
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~29 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Eq0vyEZZXJc

## ประเด็นหลัก
- ทดสอบโมเดล Qwen3.8-27B (โมเดลท้องถิ่นขนาด 27 พันล้านพารามิเตอร์) ที่รันบนเครื่อง DGX Spark กับงานท้าทายสามงาน โดยเปรียบเทียบกับ Qwen3.8-Max เวอร์ชันเต็มที่รันบนคลาวด์
- งานแรกคือการสร้างหน้าเปิดตัวเว็บไซต์ด้วย Next.js, React, TypeScript, GSAP และ Lenis smooth scrolling เวอร์ชันท้องถิ่นใช้เวลา 6.7 ชั่วโมงและได้ผลลัพธ์ดีเกินคาด ส่วนเวอร์ชัน Max ทำได้ล้ำกว่าแต่เสียค่าใช้จ่ายเกือบ $40
- โมเดลมีความสามารถด้าน vision (มองเห็นภาพ) ซึ่งเป็นข้อได้เปรียบเหนือ DeepSeek ที่ไม่มีมิติด้านภาพ ผลงานด้านภาพจึงออกมาดีมาก
- งานที่สองคือการสร้างโลก Three.js จากวรรคแรกของ Lord of the Rings ใช้เวลาเพียง 2 ชั่วโมง 17 นาที และผลลัพธ์ดีกว่าเวอร์ชันคลาวด์ของ DeepSeek อย่างชัดเจน
- งานที่สามคือการสร้างเกมแข่งรถในเบราว์เซอร์ตามภาพอ้างอิงจากเกม Days of Thunder ใช้เวลา 9 ชั่วโมง 15 นาที แต่ภาพพัง ต้องให้โมเดลอื่นตรวจสอบโค้ดและให้คำใบ้ถึงสาเหตุ
- หลังแก้ไข เกมเล่นได้ในทางเทคนิคแต่กราฟิกยังแย่ แสดงให้เห็นขีดจำกัดของโมเดล แม้ทักษะ vision จะดีแต่ก็ยังอ่าน screenshot ผิดพลาดได้
- สรุปว่าโมเดล 27B ตัวนี้ทำได้ดีเกินคาด โดยเฉพาะงานภาพ แต่การใช้งานจริงควรมี orchestrator agent (ตัวแทนผู้คอยให้ทิศทาง) หรือโมเดลที่แรงกว่าคอยช่วยเมื่อติดขัด
- ใช้ recipe จาก Unsloth (NVFP4) กับ context window 65K ที่ปรับเป็น 262K และได้ความเร็วประมาณ 12-13 tokens ต่อวินาทีบน recipe ที่ค่อนข้างเก่า
- เจ้าของช่องวางแผนทำวิดีโอเกี่ยวกับการปรับแต่ง local AI เพิ่มเติมในอนาคต และเปิดโปรเจกต์ agentwikis.com สำหรับผู้ที่สนใจ

## ความเห็นสรุป
วิดีโอนี้ให้มุมมองที่ตรงไปตรงมาและมีประโยชน์เกี่ยวกับศักยภาพและข้อจำกัดของโมเดลท้องถิ่นขนาดเล็ก แม้ Qwen3.8-27B จะยังสู้ frontier model ไม่ได้เต็มที่ แต่ก็พิสูจน์ว่าการจับคู่กับโมเดลที่ใหญ่กว่าในรูปแบบ orchestrator agent จะทำให้ใช้งานได้จริงมากขึ้น เหมาะสำหรับคนที่สนใจรันโมเดล AI ในเครื่องและอยากเห็นการทดสอบเชิงปฏิบัติมากกว่าตัวเลข benchmark ล้วนๆ

เสียงพากย์ไทย: ![[Eq0vyEZZXJc.mp3]]

