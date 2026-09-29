---
videoId: "2MdS3LuAc5w"
title: "Day 3B: Tool Calling — Complete Function Calling Guide (Gemini)"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=2MdS3LuAc5w"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 3B: Tool Calling — Complete Function Calling Guide (Gemini)

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=2MdS3LuAc5w

## 📝 สรุป

# สรุป: Day 3B: Tool Calling — Complete Function Calling Guide (Gemini)

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~21 นาที · **ลิงก์:** https://www.youtube.com/watch?v=2MdS3LuAc5w

## ประเด็นหลัก

- แม้ชื่อวิดีโอจะระบุเรื่อง Tool Calling แต่เนื้อหาจริงของ codelab นี้คือ memory management (การจัดการหน่วยความจำระยะยาว) ใน ADK — แยกจาก session ซึ่งเป็นหน่วยความจำระยะสั้นแบบบทสนทนาเดียว
- Memory ให้ความสามารถที่ session เดี่ยวๆ ทำไม่ได้: จดจำข้ามบทสนทนา สกัดข้อมูลอย่างชาญฉลาด ค้นหาเชิงความหมาย และเก็บข้อมูลถาวร
- Memory workflow มี 3 ขั้นหลัก: Initialize (สร้าง service ผ่าก runner) → Ingest (ย้ายข้อมูล session ด้วย add_session_to_memory) → Retrieve (ค้นหาด้วย search_memory)
- Notebook ใช้ InMemory memory service (จับคู่คียเวิร์ด ไม่เก็บถาวร) ส่วน production ควรใช้ Vertex AI Memory Bank (กลั่นข้อมูลด้วย LLM + semantic search + คลาวด์ถาวร) ซึ่งจะสอนใน Day 5
- การดึงข้อมูลความจำมี 2 โหมด: load_memory แบบ reactive (ทำงานเมื่อถูกเรียก) และ preload_memory แบบ proactive (เตรียมข้อมูลไว้ล่วงหน้า)
- การค้นหา memory ตั้งอยู่บนข้อเท็จจริงจริงๆ ที่เก็บไว้ เอเจนต์จึง hallucinate ความจำที่ไม่มีอยู่ไม่ได้
- Callbacks ของ ADK เป็นฟังก์ชันที่ทำงานอัตโนมัติตามจังหวะต่างๆ ของเอเจนต์ (before/after agent, before/after model, before/after tool, on model error) เหมาะกับ logging, observability และการบันทึก memory อัตโนมัติ
- ใช้ after_agent_callback + callback_context ทำ autosave บทสนทนาหลังจบทุก turn รวมกับ preload_memory ทำให้การจัดเก็บและดึงข้อมูลเป็นอัตโนมัติทั้งหมด โดยไม่ต้องเรียกด้วยมือเลย
- ความถี่ในการบันทึก memory มี 3 แบบ: ทุก turn (เรียลไทม์), หลังจบบทสนทนา (ลด API calls / batch), เป็นช่วงๆ (บทสนทนายาว)
- เก็บข้อมูลดิบทั้งหมดไม่ scale (50 ข้อความ = 10,000 tokens) — ต้องใช้ memory consolidation สกัดเฉพาะข้อเท็จจริงสำคัญทิ้ง noise ทิ้ง ผลลัพธ์คือเก็บน้อยลง ดึงเร็วขึ้น ตอบแม่นขึ้น
- Consolidation เปลี่ยนภาษาธรรมชาติเป็นข้อมูลมีโครงสร้าง เช่น "แพ้ถั่ว กินอะไรที่มีถั่วไม่ได้" → แพ้ถั่ว/ถั่วต้นไม้/หลีกเลี่ยงอย่างสมบูรณ์ และ managed service อย่าง Vertex AI ทำให้อัตโนมัติโดยใช้ API เดิม

## ความเห็นสรุป

วิดีโอนี้เดินตาม notebook ไปทีละขั้นอย่างละเอียด เหมาะกับผู้เริ่มต้นที่อยากเข้าใจว่าระบบความจำระยะยาวของเอเจนต์ทำงานอย่างไร ตั้งแต่ manual workflow ไปจนถึง automation ด้วย callbacks ครับ จุดที่ควรระวังคือชื่อวิดีโอกับเนื้อหาจริงไม่ตรงกัน (Tool Calling แต่สอน Memory) และตัวอย่างทั้งหมดใช้ InMemory service ซึ่งไม่เก็บข้อมูลถาวร ผู้ดูควรต่อยอดไปดู Day 5 เรื่อง Vertex AI Memory Bank ครับ

เสียงพากย์ไทย: ![[2MdS3LuAc5w.mp3]]

