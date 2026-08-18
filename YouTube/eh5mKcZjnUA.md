---
videoId: "eh5mKcZjnUA"
title: "Turn Local AI Into a Business with MPP (Machine Payments Protocol)"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=eh5mKcZjnUA"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# Turn Local AI Into a Business with MPP (Machine Payments Protocol)

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=eh5mKcZjnUA

## 📝 สรุป

# สรุป: Turn Local AI Into a Business with MPP (Machine Payments Protocol)
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~22 นาที · **ลิงก์:** https://www.youtube.com/watch?v=eh5mKcZjnUA

## ประเด็นหลัก
- MPP (Machine Payments Protocol) คือมาตรฐานเปิดที่พัฒนาโดย Stripe และ Tempo ให้ AI agent จ่ายเงินรายเล็กได้เองโดยไม่ต้องอาศัยฟอร์มชำระเงินแบบมนุษย์
- ภาพเปิดวิดีโอถูกสร้างด้วยโมเดล Coya 2 บน DGX Spark ของคนอื่น โดยจ่ายเพียงเศษเสี้ยวเซนต์ผ่าน MPP — เป็นตัวอย่าง "เช่าโมเดล" ข้ามเครื่อง
- ต้นกำเนิดมาจากรหัส HTTP 402 (payment required) ที่สงวนไว้ตั้งแต่ปี 1997 ถูกฟื้นเป็น X402 ในวงการบล็อกเชน แล้วอัปเกรดเป็น MPP ในเดือนมีนาคมปีนี้
- กลไกการทำงาน: agent ขอทรัพยากร → ได้รับบิลแยกรายการ → จ่ายเงิน (stablecoin หรือบัตรเครดิต) → โชว์ใบเสร็จ → ได้สิทธิ์เข้าถึง ไม่ต้องมีบัญชีหรือ API key
- การชำระเงินมี 3 รูปแบบ: แบบเครื่องขายของอัตโนมัติ (จ่ายต่อหน่วย), แบบบาร์แท็บ (เปิดแท็บเดียวรันหลายพันรายการ เหมาะกับ MPP), และแบบสมาชิก
- รองรับ 10 วิธีชำระเงินตามสเปก มากกว่า 15 chains ผ่านปลั๊กอินชุมชน และเครื่องมือกว่า 100 รายการในระบบนิเวศ
- การสาธิตจริง: ตั้ง MPP gateway บน DGX Spark ด้วย Ollama + Qwen 3 coder และ ComfyUI + Coya 2 เปิดผ่าน ngrok ราคา 1 เซนต์ต่อภาพ ฝาก 10 เซนต์แล้วสร้างภาพมังกรในโลกบอนไซได้ 6 ภาพ เหลือ 4 เซนต์คืนเมื่อปิดเซสชัน
- ข้อจำกัด: ยังเป็นมาตรฐานฉบับร่าง ราคาต่ำกว่าเซนต์ต้องอาศัยวอลุ่ม ต้องตั้ง rate limit ดูแล GPU เก็บ payout keys ให้ปลอดภัย และไม่มีระบบคืนเงินหากถูกหลอก
- ไอเดียธุรกิจ: เปลี่ยนโมเดล AI ที่รันในเครื่องให้กลายเป็นบริการสร้างภาพ/วิดีโอที่คนอื่นจ่ายเงินใช้ได้ โดยโปรโตคอลเองทำหน้าที่เป็นระบบบิลลิง

## ความเห็นสรุป
วิดีโอนี้ให้ภาพรวม MPP ที่เข้าใจง่ายทั้งภาคทฤษฎีและปฏิบัติจริง พร้อมเดโม่ที่พิสูจน์ว่า "โมเดลในบ้านสร้างรายได้" เป็นไปได้จริงบน testnet แม้ผู้พูดจะยอมรับตรง ๆ ว่าระบบยังตั้งค่าลำบากและต้องอาศัยวอลุ่มถึงจะคุ้ม แต่แนวคิดการเปลี่ยน local AI ให้เป็นบริการผ่าน micropayment ถือเป็นทิศทางที่น่าจับตามองในเศรษฐกิจแบบ agent-to-agent

เสียงพากย์ไทย: ![[eh5mKcZjnUA.mp3]]

