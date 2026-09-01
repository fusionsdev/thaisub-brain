---
videoId: "VratNtvAMeA"
title: "Breaking Down Kimi K3's Architecture (Even For the Non-Technical)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=VratNtvAMeA"
published: "2026-07-23"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Breaking Down Kimi K3's Architecture (Even For the Non-Technical)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=VratNtvAMeA

## 📝 สรุป

# สรุป: Breaking Down Kimi K3's Architecture (Even For the Non-Technical)

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~25 นาที · **ลิงก์:** https://www.youtube.com/watch?v=VratNtvAMeA

## ประเด็นหลัก

- **Kimi K3** เป็นโมเดล open weights ที่ใหญ่ที่สุดเท่าที่เคยปล่อยมา ที่ขนาด 2.8 ล้านล้านพารามิเตอร์ แต่กลับทำงานได้ถูกกว่าโมเดลที่เล็กกว่าหลายเท่า
- สถาปัตยกรรมของ Kimi K3 มีเทคนิคลดต้นทุนแยกกัน 4 จุด ได้แก่ การอ่านคำถาม, การคิด, การเขียนคำตอบ, และการเทรนโมเดล
- **Mixture of Experts (MoE):** จาก 896 expert จะเลือกมาใช้แค่ 16 คนต่อครั้ง ทำให้ได้ความรู้ของโมเดลยักษ์ในราคาโมเดลเล็ก
- **Quantile Balancing:** กระจายงานระหว่าง expert อัตโนมัติ ไม่ต้องปรับค่า magic number ทำให้สามารถใช้ MoE แบบ 16/896 ได้โดยไม่พัง
- **Kimi Delta Attention (KDA):** ใช้ whiteboard ขนาดคงที่แทนการเก็บทุก token โดยมีการ "เช็ดก่อนเขียน" ทำให้ต้นทุนไม่เพิ่มตามความยาว context
- **Gated MLA:** สถานี full transcript ที่กระจายอยู่ใน layer stack ทำหน้าที่เป็น safety net ให้ความแม่นยำ
- **Attention Residuals:** นวัตกรรมของ Kimi K3 ที่ให้ layer เลือกดึงข้อมูลจาก layer อื่นๆ แบบตั้งฉาก ลดการเจือจางของข้อมูล
- **4-bit Quantization (MX FP4):** ลดขนาด weight จาก 5.5 terabytes เหลือ 1.4 terabytes ทำให้คลังเล็กลง เข้าถึงได้เร็วขึ้น
- **QAT from SFT:** โมเดลเรียนรู้ในรูป 4-bit ตั้งแต่ต้น ทำให้การบีบอัดไม่ทำลายคุณภาพ
- **Per-head Muon:** เทรนแต่ละส่วนของ attention แยกจากกัน เป็นอีกหนึ่งนวัตกรรมของ Kimi K3
- การประหยัดจากทุกเทคนิคไม่ได้แค่บวกกัน แต่คูณกัน เพราะแต่ละเทคนิคโจมตีคนละคอขวด

## ความเห็นสรุป

Kimi K3 แสดงให้เห็นว่าอนาคตของ AI ไม่ใช่แค่โมเดลที่ใหญ่ขึ้นอย่างเดียว แต่เป็นโมเดลที่รู้ว่าควรข้ามอะไรไปบ้างเพื่อให้ทำงานได้มีประสิทธิภาพและประสิทธิผลสูงสุดครับ สถาปัตยกรรมแบบผสมที่ออกแบบมาอย่างแนบเนียนนี้ ทำให้ Kimi K3 กลายเป็นโมเดลที่น่าจับตามองมากครับ

เสียงพากย์ไทย: ![[VratNtvAMeA.mp3]]
