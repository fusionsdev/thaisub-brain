---
videoId: "upI7bqagxLY"
title: "Making an Animated Short with Free AI Tools (Part 1. MiniMax H3 Video Gen)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=upI7bqagxLY"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-11"
tags: [thai-sub, youtube]
---

# Making an Animated Short with Free AI Tools (Part 1. MiniMax H3 Video Gen)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=upI7bqagxLY

## 📝 สรุป

# สรุปภาษาไทย — Making an Animated Short with Free AI Tools (Part 1)

**ช่อง:** Tonbi's AI Garage · **เผยแพร่:** 5 ตุลาคม 2026 · **ความยาว:** 38:12

---

## ใจความสำคัญ

Tonbi ทดลองสร้างแอนิเมชันสั้นแนวดิ่งความยาวไม่เกิน 1 นาที โดยใช้เครื่องมือ AI ฟรีทั้งหมด แรงบันดาลใจมาจากคลิปไวรัล 13 ล้านวิวของ Turpp ที่ใช้สไตล์ Pixar

**เครื่องมือหลัก:** MiniMax H3 (โอเพนซอร์ส, รันบนเครื่องตัวเอง), Grok 4.7 / GPT-4o 6.1 สำหรับช่วยวางแผนและเขียนพรอมต์, Hyperframes (ใช้ใน Part 2 สำหรับทำ caption), Hermes Desktop สำหรับจัดการ session

## เนื้อเรื่อง

เป็นเรื่องล้อเลียนเชิงเสียดสีเกี่ยวกับ local AI — ตัวละครหนุ่มอยากซื้อ GPU แต่แฟนบอกว่า "Local AI มันไร้ประโยชน์" คืนนั้นเขาฝันเห็นโลกอนาคตที่ทุกคนถูกบังคับให้สร้างแค่ "กล่องสีเทา" ในโรงงาน ห้ามใช้ความคิดสร้างสรรค์เพราะ "ความปลอดภัย" (ล้อเลียนนโยบายเซ็นเซอร์ของบริษัท AI ใหญ่) เขาเห็นคนที่มี GPU ของตัวเองสามารถสร้างไดโนเสาร์สีสันและอะไรเจ๋งๆ ได้อย่างอิสระ ตื่นมาเขาก็เดินไปซื้อ GPU ทันที

## กระบวนการสร้าง (2 วันเต็ม)

1. **วางแผนเรื่องและ beat sheet** — เขียนบททีละจังหวะ
2. **ออกแบบตัวละครด้วย image generation** — พยายามรักษา consistency ระหว่าง local model
3. **สร้าง key frames** — ฉากสำคัญแต่ละฉาก
4. **Video generation ด้วย MiniMax H3** — 884 segments, แต่ละคลิปใช้เวลา ~20 นาที
5. **เสียงพูด** — H3 สร้างเสียงให้ตัวละคร ยกเว้นพนักงานที่ Tonbi พากย์เอง
6. **Part 2 (แยกวิดีโอ):** ตัดต่อ + Hyperframes caption + outro + โพสต์ X

## ปัญหาที่พบ

- **Consistency:** รักษาหน้าตัวละครให้เหมือนเดิมทุกฉากยากมาก โดยเฉพาะเมื่อใช้ local model
- **Face drift:** ฉากที่แพนออกไกลๆ หน้าคนเพี้ยน
- **Object consistency:** ฝากล่องโผล่ๆ หายๆ ต้องเจนซ้ำหลายรอบ
- **เสียงไม่ consistent:** เสียงพนักงานเปลี่ยนไปในแต่ละคลิป

## เทคนิคที่ใช้

- ฉากสั้น (~3 วิ) สลับไปมาเพื่อลด drift
- ใช้ reference condition จาก H3 เพื่อล็อกหน้าตัวละคร
- ไม่วาดคำลงในภาพ — ทำ caption ทีหลังใน Hyperframes
- เร่งความเร็วคลิปใน post-production

## สรุป

ถึงแม้จะใช้เวลา 2 วันเพื่อสร้างวิดีโอไม่ถึง 1 นาที Tonbi บอกว่า workflow โดยรวมค่อนข้าง smooth และสามารถ streamline ได้อีกถ้าอยากทำเป็นประจำ

เสียงพากย์ไทย: ![[upI7bqagxLY.mp3]]

