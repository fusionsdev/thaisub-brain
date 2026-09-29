---
videoId: "r3GDPvlVZXg"
title: "Day 5A: AI Agent Deployment — Running Agents in Production"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=r3GDPvlVZXg"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 5A: AI Agent Deployment — Running Agents in Production

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=r3GDPvlVZXg

## 📝 สรุป

# สรุป: Day 5A: AI Agent Deployment — Running Agents in Production

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~15 นาที · **ลิงก์:** https://www.youtube.com/watch?v=r3GDPvlVZXg

## ประเด็นหลัก

- Assignment สุดท้ายของคอร์ส หัวข้อ prototype to production — เนื้อหาหลักคือ A2A protocol (agent-to-agent) สำหรับให้เอเจนต์อิสระหลายตัวสื่อสารและร่วมมือกันข้ามเครือข่ายและ framework
- เอเจนต์เดี่ยวทำทุกอย่างไม่ได้: ทีมต่างๆ สร้างเอเจนต์ต่างกัน ใช้ภาษา/framework ต่างกัน จึงต้องมีโปรโตคอลสื่อสารมาตรฐาน — A2A คือคำตอบ
- จุดเด่นของ A2A: เรียกเอเจนต์อื่นเหมือนเรียก tool, framework/language agnostic, รักษาสัญญาที่เป็นทางการผ่าน agent cards
- กรณีใช้งานหลัก 3 แบบ: cross framework (ADK ↔ framework อื่น), cross language (Python เรียก Java/Node.js), cross organization (เอเจนต์ภายใน ↔ service ผู้ให้บริการภายนอก)
- ตัวอย่างใน codelab: product catalog agent (ฝั่งผู้ขายภายนอก ให้ข้อมูลสินค้า) และ customer support agent (ฝั่งเรา ตอบลูกค้า) — จำลองรันบน localhost เพื่อการเรียน ใน production จะรันคนละโครงสร้างพื้นฐานแล้วคุยกันผ่านเน็ต
- ขั้นตอน 6 ขั้น: สร้าง product catalog agent → เปิดเผยผ่าน A2A → เริ่ม server → สร้าง customer support agent → ทดสอบการสื่อสาร → เข้าใจ flow
- Agent card = นามบัตร JSON ของเอเจนต์ (ชื่อ คำอธิบาย เวอร์ชัน skills URL endpoints) เผยแพร่ที่ path มาตรฐาน well-known/agent-card.json — ทุกเอเจนต์ A2A ต้องมี
- การเปิดเผย ADK agent ผ่าน A2A ทำได้ง่ายที่สุดด้วยฟังก์ชัน A2A ของ ADK: ห่อเอเจนต์ใน server ที่เข้ากันได้ (FastAPI/Starlette + uvicorn) แล้วสร้าง agent card อัตโนมัติ
- Flow การทำงาน: ลูกค้าถาม → support agent มอบหมายให้ sub-agent (remote A2A proxy) → ส่ง A2A request ผ่าน HTTP → catalog agent เรียก get_product_info → ตอบกลับ → support agent ประกอบคำตอบสุดท้ายให้ลูกค้า
- การใช้งานจริง: microservices, การเชื่อมบุคคลที่สาม, cross language, cross organization; ไอเดียต่อยอด: เพิ่ม inventory/shipping agent + coordinator, ใช้ฐานข้อมูลจริง (MongoDB), เชื่อม payment gateway จริง
- ขั้นถัดไป (optional): deploy product catalog agent ขึ้น Vertex AI Agent Engine บน Google Cloud แล้วอัปเดต URL ใน agent card เป็น production server จริง

## ความเห็นสรุป

วิดีโอนี้อธิบาย A2A ได้กระชับและเป็นรูปเป็นร่าง ผ่านตัวอย่าง e-commerce ที่รันได้จริงบน localhost ครับ จุดที่ควรเก็บคือแนวคิด agent card และการที่ remote agent ถูกมองเป็น sub-agent ผ่าน proxy ทำให้โค้ดฝั่งผู้ใช้เขียนเหมือนใช้เอเจนต์ local ทั่วไปครับ ชื่อวิดีโอ ("Deployment — Running Agents in Production") สื่อกว้างกว่าเนื้อหาจริงซึ่งเจาะ A2A เป็นหลัก ส่วน deployment จริงบน Agent Engine ถูกพูดถึงเพียงสั้นๆ ตอนท้ายครับ

เสียงพากย์ไทย: ![[r3GDPvlVZXg.mp3]]

