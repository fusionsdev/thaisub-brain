---
videoId: "xYAOR5bew8g"
title: "Exploring Hermes MoA: Is the Agg Or Ref Model More Important?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=xYAOR5bew8g"
published: "2026-07-15"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Exploring Hermes MoA: Is the Agg Or Ref Model More Important?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=xYAOR5bew8g

## 📝 สรุป

# สรุป: Exploring Hermes MoA: Is the Agg Or Ref Model More Important?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~14 นาที · **ลิงก์:** https://www.youtube.com/watch?v=xYAOR5bew8g

## ประเด็นหลัก

- วิดีโอนี้ทดลองเปรียบเทียบ Mixture of Agents (การรวมหลายโมเดลเข้าด้วยกัน) ใน Hermes Agent โดยใช้ชุดประเมิน (benchmark suite) ที่สร้างขึ้นเอง ประเมิน 5 แกน: ความเร็ว, tool calls, reasoning, instruction following และการสร้าง landing page
- การให้คะแนนเป็นแบบ deterministic Python (ไม่มี LM judge ตรวจการบ้านตัวเอง) เทียบเท่ากันทุกโปรไฟล์ ใช้ benchmark สำคัญเช่น BFCL (Berkeley Function Calling) และ IFEval
- การทดลองหลัก: ใช้ Mixtral 8x7B Pro เป็น aggregator กับ DeepSeek V4 Flash เป็น reference (AggRef-Mixtral) แล้วสลับเป็น DeepSeek เป็น aggregator กับ Mixtral เป็น reference (AggRef-DeepSeek)
- ผลการทดลอง AggRef-Mixtral ได้คะแนนรวม 92% ส่วน AggRef-DeepSeek ต่ำกว่าเล็กน้อย แม้จะเร็วกว่าอย่างมากและทำ landing page ได้สไตล์ดีกว่า
- การรันโมเดลเดี่ยวเปรียบเทียบกับ MoA: Mixtral เดี่ยวได้ 92%, DeepSeek เดี่ยวได้ 76% แต่เมื่อใช้ Mixtral เป็น reference กับ DeepSeek aggregator ดึงคะแนนขึ้นเป็น 84%
- สรุปสำคัญ: aggregator สำคัญกว่า reference — ถ้าให้เลือก ควรใส่โมเดลที่ก้าวหน้ากว่าเป็น aggregator เพื่อผลลัพธ์ที่ดีกว่า ส่วน reference ช่วยเสริมขีดความสามารถ
- MoA มีประสิทธิภาพจริงในการดึงโมเดลที่อ่อนกว่าให้ทำได้ดีขึ้น โดยเฉพาะเมื่อได้รับคำแนะนำจากโมเดลที่แข็งแกร่งกว่า
- เอเจนต์ reference ทำหน้าที่เหมือน "โค้ช" คอยจับบั๊ก/ความเสี่ยง และ aggregator ก็ให้เครดิต reference ที่จับปัญหาได้
- สไตล์การสร้าง landing page แตกต่างกันตามโมเดลที่เป็นหลัก: DeepSeek ใช้สีเข้มและหัวเรื่องคล้ายกัน ส่วน Mixtral ใช้คำที่ต่างออกไป
- คำถามติดตามที่จะทำวิดีโอถัดไป: จำนวน reference models ที่เหมาะสมคือเท่าไหร่? และกลุ่มโมเดลฟรีสู้โมเดลเสียเงินตัวเดียวได้หรือไม่?
- เอเจนต์สามารถเห็น "ความคิด" ของ reference model ได้แบบเรียลไทม์ ซึ่งเป็นฟีเจอร์ใหม่ที่ผู้จัดไม่เห็นในการรันก่อนหน้า

## ความเห็นสรุป

วิดีโอนี้ให้ข้อสรุปที่ชัดเจนว่าใน Mixture of Agents บทบาท aggregator สำคัญกว่า reference — ควรใส่โมเดลที่ดีกว่าเป็น aggregator เพื่อผลลัพธ์ที่ดีที่สุด แม้จะเสียเวลามากกว่า ในขณะที่ reference model ช่วยยกระดับโมเดลที่อ่อนกว่าได้อย่างมีประสิทธิภาพ ผลการทดลองแสดงให้เห็นว่า MoA ไม่ใช่แค่ทฤษฎี แต่ใช้งานได้จริงในการสร้างโมเดลที่ทรงพลังกว่าโมเดลเดี่ยว

เสียงพากย์ไทย: ![[xYAOR5bew8g.mp3]]
