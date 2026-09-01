---
videoId: "KtlY6ETPyKo"
title: "Hermes Agent Masterclass: 10. Security"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=KtlY6ETPyKo"
published: "2026-07-10"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Hermes Agent Masterclass: 10. Security

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=KtlY6ETPyKo

## 📝 สรุป

# สรุป: Hermes Agent Masterclass: 10. Security

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~28 นาที · **ลิงก์:** https://www.youtube.com/watch?v=KtlY6ETPyKo

## ประเด็นหลัก

- วิดีโอนี้เป็นตอนจบของซีรีส์ Hermes Agent Masterclass ทั้ง 10 ตอน โดยเน้นเรื่องความปลอดภัย (Security) ของ agent
- ไม่มี agent ที่ปลอดภัยและมีความสามารถสูงสุดพร้อมกันได้ — ต้องเลือก trade-off ระหว่างความสามารถกับความปลอดภัยให้เหมาะกับงาน
- 7 ชั้นความปลอดภัยทำงานเป็น "dial" หรือปุ่มปรับระดับ ไม่ใช่ checklist ที่ต้องเปิดให้หมด
- Trust Layer: ใครสามารถคุยกับ agent ได้บ้าง — ค่าเริ่มต้นคือปฏิเสธทุกคน (deny by default)
- Approvals: มีหลายโหมด — Manual, Smart (LLM ประเมินความเสี่ยง), และ YOLO (ทำทุกอย่างไม่ต้องถาม)
- แม้ใน YOLO mode ก็มี hard block สำหรับคำสั่งที่อันตรายระดับหายนะ เช่น `rm -rf /`
- Containment: ใช้ Docker เป็น boundary — host file system ไม่ถูกเข้าถึงได้ แต่ต้องระวัง ENV ที่ forward เข้า container
- Filtering: MCP เห็น secret น้อยมาก ทุกอย่างถูก strip/redact ก่อนถึง LLM
- ไฟล์เองก็โจมตีคุณได้ (prompt injection) — agents.md, soul.md ฯลฯ ถูก scan ก่อน load
- SSRF protection และ website block list ทำงานตลอดเวลาที่ network level
- Tyrith/Teereth: เครื่องมือ pre-exec scanning จับ homograph URL spoofing และ Unicode look-alike attacks
- ทุกชั้นความปลอดภัยปรับได้ตาม profile (agent แยกกัน) เพื่อให้แต่ละ agent มีสิทธิ์น้อยที่สุดเท่าที่งานต้องการ

## ความเห็นสรุป

วิดีโอนี้เป็นบทสรุปที่ครอบคลุมและเป็นประโยชน์มาก แสดงให้เห็นว่า Hermes Agent ออกแบบมาด้วย defense in depth 7 ชั้นที่ซ้อนทับกัน ผู้ใช้สามารถปรับแต่งระดับความปลอดภัยได้ตามความเหมาะสม ตั้งแต่ใช้คนเดียวบนแล็ปท็อปไปจนถึงการ deploy สาธารณะ เป็นการปิด Masterclass ได้อย่างสมบูรณ์และทรงพลังครับ

เสียงพากย์ไทย: ![[KtlY6ETPyKo.mp3]]
