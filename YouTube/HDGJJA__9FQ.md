---
videoId: "HDGJJA__9FQ"
title: "Beginner's Guide to Agent Wikis"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=HDGJJA__9FQ"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-11"
tags: [thai-sub, youtube]
---

# Beginner's Guide to Agent Wikis

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=HDGJJA__9FQ

## 📝 สรุป

# สรุปภาษาไทย — Beginner's Guide to Agent Wikis

> **ที่มา:** [YouTube — Tonbi's AI Garage](https://www.youtube.com/watch?v=HDGJJA__9FQ) · เผยแพร่ 10 ก.ย. 2026 · ~13:46 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Tonbi's AI Garage*

## วิดีโอนี้เกี่ยวกับอะไร

คู่มือสำหรับมือใหม่เกี่ยวกับ **Agent Wikis** เว็บฐานความรู้สไตล์วิกิที่เจ้าของช่องสร้างไว้ให้เอเจนต์ AI ใช้ตอบคำถามจากข้อมูลที่สังเคราะห์แล้ว แทนการค้นเว็บใหม่ทุกครั้ง โดยสาธิตวิธีติดตั้งผ่าน **MCP server** เทียบประสิทธิภาพกับ web search ธรรมดา แล้วปิดท้ายด้วยฟีเจอร์ของ **pro tier**

## ประเด็นหลัก

1. **Agent Wikis คืออะไร:** ฐานความรู้สไตล์วิกิที่เอเจนต์ถามตอบโดยอ้างอิงเนื้อหาในวิกิ ถ้าตอบไม่ได้ก็ไปค้นเว็บแล้วเอากลับมาเพิ่มลงวิกิ แนวคิดเดียวกับที่ Andre Karpathy โพสต์เรื่อง LM knowledge bases จนเป็นไวรัล
2. **จุดเริ่มต้นแบบโอเพนซอร์ส:** เทมเพลตฟอร์แมต LM Wiki เปิดไว้บน GitHub ของ Toby Studio ใครก็เอาไปสร้างวิกิของตัวเองได้ ก่อนจะรวมมาเป็นเว็บ agentwiks.com แทนการกระจายตาม repo
3. **ทำไมถึงดี:** ยกตัวอย่างซีรีส์ Hermes Agent Masterclass ที่สร้างจาก knowledge base ของ Hermes Agent ทั้งชุด ได้คำตอบละเอียดและเร็วขึ้น ภาพหลอนน้อยลง ใช้ token น้อยลง เพราะคอมไพล์ครั้งเดียวแล้วถามซ้ำได้หลายเดือน
4. **ตัวเว็บออกแบบให้เอเจนต์ใช้:** ทุกหน้ามี llms.txt เป็นจุดเริ่มต้นมาตรฐาน มี raw markdown ให้อ่าน เนื้อหาสังเคราะห์จากเอกสารทางการกับ repo กับ issue และแหล่งคอมมูนิตี้อย่าง Reddit เพื่อเก็บทั้งวิธีใช้ทางการและจุดที่คนมักพลาด
5. **วิธีใช้ผ่าน MCP:** สาธิตกับเอเจนต์บน DGX Spark ที่ไม่เคยใช้มาก่อน สั่งให้ไปที่ agentwiks.com แล้วติดตั้ง MCP server เครื่องมือมีแค่ list wikis กับ open wiki กับ search และ read document แล้วถามเรื่อง hyperframe shader effects ได้คำตอบว่าเป็น WebGL fragment shaders ไม่ใช่ CSS พร้อมแยกสามเลเยอร์
6. **เทียบกับ web search:** ถามเรื่องสามฟีเจอร์ของ Hermes Agent bot mode กับหนึ่ง gotcha แบบใช้ web search ล้วนใช้ context ราว 59.3K tokens ส่วนผ่าน Agent Wikis MCP ใช้แค่ราว 27.8K tokens ได้คำตอบครบเหมือนกัน แถมวิกิกล้าตอบว่าไม่รู้แทนการตอบผิดอย่างมั่นใจ
7. **ราคาและการใช้งาน:** ตัววิกิกับ MCP server ใช้ฟรีและอัปเดตให้ฟรี เว็บมีวิกิเกิน 60 ตัว ส่วน pro tier ตอนนี้เดือนละ 9.99 ดอลลาร์ วันที่ 1 ตุลาคมจะขึ้นเป็น 19.99 ดอลลาร์ สมัครก่อนล็อกราคาเดิม
8. **ของใหม่ใน pro tier:** XL Wikis ที่ใหญ่และลึกกว่าขนาดมาตรฐาน กับ custom skills ที่เป็นสกิลจริงจากงานของเจ้าของช่อง ทั้งสาย hyperframes กับ local AI กับ DGX Spark กับ generative media และ scroll film engineering ติดตั้งด้วยไฟล์ tar.gz บวก API key ใน ENV file แล้วกำลังจะตามด้วย custom profiles อย่าง onchain analyst กับสายวิดีโอโปรดักชันและ custom workflows

## ใครควรดู

คนที่รันเอเจนต์ AI เป็นประจำและอยากได้คำตอบที่นิ่งกว่า web search รวมถึงคนที่สนใจสร้าง knowledge base ของตัวเองหรืออยากดูว่า pro tier ของ Agent Wikis คุ้มหรือไม่

---
*Attribution: Beginner's Guide to Agent Wikis — Tonbi's AI Garage (youtube.com/watch?v=HDGJJA__9FQ), เผยแพร่ 10 ก.ย. 2026*

เสียงพากย์ไทย: ![[HDGJJA__9FQ.mp3]]

