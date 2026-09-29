---
videoId: "KgUsl7UGGFA"
title: "Day 2A: Agent Tools — How AI Agents Use Tools (Hands-On Demo)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=KgUsl7UGGFA"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 2A: Agent Tools — How AI Agents Use Tools (Hands-On Demo)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=KgUsl7UGGFA

## 📝 สรุป

# สรุป: Day 2A: Agent Tools — How AI Agents Use Tools (Hands-On Demo)
- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~26 นาที · **ลิงก์:** https://www.youtube.com/watch?v=KgUsl7UGGFA

## ประเด็นหลัก
- แบบฝึกหัด Day 2 Part A ของคอร์ส Google × Kaggle 5-Day AI Agents Intensive พาทำ code lab บน Kaggle notebook ด้วย Google ADK
- Custom tool คือ Python function ที่แปลงเป็น agent tool เพื่อรองรับ business logic เฉพาะของเรา ซึ่ง built-in tool แบบ generic ตอบโจทย์ไม่ได้
- แนวปฏิบัติที่ดีเวลาเขียน function tool: return เป็น dictionary มี status, docstring ชัดเจน, ใส่ type hints และมี error handling
- ตัวอย่างหลักคือ currency converter agent ที่ใช้ tool สองตัว คือ get_fee_for_payment_method (หาค่าธรรมเนียม) และ get_exchange_rate (ดึงอัตราแลกเปลี่ยน)
- ให้ agent สร้าง Python code แล้วรันผ่าน built-in code executor น่าเชื่อถือกว่าปล่อยให้ LLM คิดเลขเอง เพราะ LLM อาจคำนวณผิดหรือใช้สูตรไม่สอดคล้อง
- Calculation agent ถูกออกแบบให้ตอบกลับเป็น Python code เท่านั้น แล้วใช้ code execution ของ Gemini รันใน sandbox โดยไม่ต้องมี production environment
- ความต่างสำคัญ: agent tool คือการ agent A เรียก agent B เป็นเครื่องมือ แล้ว B ตอบกลับมาที่ A ซึ่ง A ยังคุมบทสนทนาต่อ (ใช้กรณี delegation)
- Sub-agent คือการโอนการควบคุมทั้งหมดให้ agent B แล้ว B รับช่วงดูแลผู้ใช้ต่อเอง (ใช้กรณี handoff) เช่น ชั้น level 1/2/3 ของฝ่าย support
- ภาพรวม tool ของ ADK แบ่งเป็น custom (function tool, long-running function tool, agent tool, MCP tool, OpenAPI tool) และ built-in (Gemini tool, Google tool เช่น BigQuery, third-party tool เช่น GitHub และ Hugging Face)
- MCP tool เชื่อมบริการที่รองรับ MCP ได้ทันทีโดยไม่ต้องเขียน integration เอง ส่วน OpenAPI tool เปลี่ยน REST API endpoint ให้กลายเป็น tool ที่เรียกใช้ได้ ด้วยการให้ API spec อย่างเดียว

## ความเห็นสรุป
วิดีโอนี้เหมาะกับผู้เริ่มต้นสร้าง agent ด้วย Google ADK เพราะเดินตาม code lab ทีละขั้นตอนแบบละเอียด ตั้งแต่เตรียม environment จนถึงภาพรวม tool ทั้งหมด จุดเด่นคือตัวอย่าง currency converter ที่ต่อยอดจาก tool ธรรมดาไปเป็น multi-tool agent พร้อม calculation agent แบบ step by step ทำให้เห็นภาพการใช้งานจริงชัดเจน และคำอธิบายเรื่อง agent tool กับ sub-agent ที่เทียบกับ pattern จาก Day 1 ช่วยให้เข้าใจความต่างของการควบคุมบทสนทนาได้ดีมากครับ

เสียงพากย์ไทย: ![[KgUsl7UGGFA.mp3]]

