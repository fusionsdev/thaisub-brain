---
videoId: "UewPtE0rMP4"
title: "Buzz Workflows Guide: Easily Create Agent Automations"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=UewPtE0rMP4"
published: "2026-10-26"
has_voiceover: true
status: translated
synced_at: "2026-10-27"
tags: [thai-sub, youtube]
---

# Buzz Workflows Guide: Easily Create Agent Automations

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=UewPtE0rMP4

## 📝 สรุป

# สรุปภาษาไทย — Buzz Workflows Guide: Easily Create Agent Automations

> **ที่มา:** [YouTube — Tonbi's AI Garage](https://www.youtube.com/watch?v=UewPtE0rMP4) · เผยแพร่ 26 ต.ค. 2026 · ~12:53 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Tonbi's AI Garage*

## วิดีโอนี้เกี่ยวกับอะไร
อัปเดตฟีเจอร์ใหม่ของ **Buzz** (แอป agent chat ของทีม Block) นั่นคือ **workflows** — automation แบบ visual editor ที่รันบน relay ได้แม้ปิดแล็ปท็อป และปลุกเอเจนต์ให้ทำงานได้ เหมาะกับทีมและ community มากกว่าสายลุยเดี่ยว

## ประเด็นหลัก

1. **workflows คืออะไร:** automation ที่มีชื่อ + trigger (ตัวจุด) + ขั้นตอนตามลำดับ ผูกกับหนึ่ง channel ตัว relay เป็นคนรัน ไม่ใช่เครื่องของคุณ
2. **เปิดฟีเจอร์:** เป็น experimental ต้องเปิดที่ settings → experiments ก่อน (สาธิตบนเวอร์ชัน 0.5.28) เมนู workflows จะโผล่ใต้ agents
3. **5 trigger:** message posted (กรองด้วย filter ได้) / reaction added (เจาะจงอีโมจิได้) / schedule (cron time หรือ interval เช่นทุก 30 นาที) / webhooks (รับ HTTP POST จาก service ภายนอก) / diff posted (สำหรับ coding agent)
4. **7 action:** ใช้ได้จริงตอนนี้คือ send message, call web hook, delay ส่วน add reaction / send DM / set channel topic / request approval ยังมีปัญหาบ้าง
5. **เดโม 1 — message trigger:** ข้อความจากตัวเองที่มีคำว่า "go" → บอทตอบกลับทันที
6. **เดโม 2 — schedule ปลุกเอเจนต์:** ทุก 15 นาทีส่ง "@fizz research and summarize the latest AI model releases" แล้วเอเจนต์ Fizz ตื่นมาทำงานและตอบผลใน channel เหมือน cron job
7. **เดโม 3 — webhook จดหมายข่าว:** สร้าง webhook URL + private secret (โชว์ครั้งเดียว) ผูกกับ Beehiiv ที่ onchain.com เมื่อมีคนสมัครใหม่ ข้อความ "new subscriber" โผล่ใน channel ทันที
8. **ข้อควรรู้:** สมาชิก channel สร้าง workflow ได้ แต่เรียก webhook ต้องมีสิทธิ์ระดับ admin · รันพร้อมกันได้ 100 run ต่อ relay · webhook ต้องเป็น public https เท่านั้น · มีการ์ดกัน self-trigger ไม่ให้วนลูป · ทำผ่าน CLI ได้นอกจากในแอป
9. **มุมผู้สร้าง:** ดีมากสำหรับคนไม่สายเทคนิคที่อยากได้ automation แบบที่ปกติต้องเขียนเองใน Hermes agent — สร้างเสร็จในราว 1 นาที เพิ่มได้หลาย step และแชร์กันได้

## ใครควรดู
ผู้ใช้ Buzz / ทีมและ community ที่อยากได้ automation ปลุกเอเจนต์อัตโนมัติโดยไม่ต้องเขียนโค้ด

---
*Attribution: Buzz Workflows Guide: Easily Create Agent Automations — Tonbi's AI Garage (youtube.com/watch?v=UewPtE0rMP4), เผยแพร่ 26 ต.ค. 2026*

เสียงพากย์ไทย: ![[UewPtE0rMP4.mp3]]

