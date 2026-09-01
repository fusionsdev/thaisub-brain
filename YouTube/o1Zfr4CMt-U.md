---
videoId: "o1Zfr4CMt-U"
title: "Testing Moshi: SSH Client Mobile App Designed for Coding Agents"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=o1Zfr4CMt-U"
published: "2026-07-28"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Testing Moshi: SSH Client Mobile App Designed for Coding Agents

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=o1Zfr4CMt-U

## 📝 สรุป

# สรุป: Testing Moshi: SSH Client Mobile App Designed for Coding Agents

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~17 นาที · **ลิงก์:** https://www.youtube.com/watch?v=o1Zfr4CMt-U

## ประเด็นหลัก

- **Moshi** เป็นแอป mobile terminal สำหรับ iOS และ Android ที่ออกแบบมาเพื่อควบคุม AI coding agents โดยเฉพาะ ไม่ใช่แค่ SSH client ทั่วไป
- แอปพัฒนาโดย Joel (Indie Joe) บน Twitter โดยมีแนวคิดคล้าย Herder ที่เป็น agent-first tmux — Moshi จึงเป็น agent-first mobile SSH client
- รองรับการเชื่อมต่อผ่าน SSH, mosh protocol และ terminal ไปยังเครื่องที่ผู้ใช้มีอยู่แล้ว (เช่น NVIDIA DGX Spark)
- session อยู่ใน tmux/Herder/Zellij ทำให้ agents ทำงานต่อได้แม้แอปอยู่เบื้องหลังหรือเครือข่ายสลับ
- ฟีเจอร์เด่น: agent inbox, voice input, image paste เข้า prompt, mosh hook สำหรับรับเหตุการณ์ของ agent
- เปรียบเทียบกับ Termius: Moshi เน้นควบคุม agent จากระยะไกล ส่วน Termius เน้นการจัดการเซิร์ฟเวอร์และ SSH connections ที่กว้างกว่า
- การติดตั้งง่ายมาก ใช้ easy pair QR code เชื่อมต่อกับ host ได้ในคลิกเดียว ง่ายกว่า Termius
- ทดสอบจริงร่วมกับ Herder บน Spark: สามารถสลับระหว่าง Claude, Codex, Grok, Hermes ได้อย่างลื่นไหล ไม่แล็ก
- ฟังก์ชัน hooks สามารถแสดงเหตุการณ์ของ agent บนหน้าจอล็อกของ iOS (live activity) และอนุมัติ tool calls ได้จากหน้าจอล็อกโดยตรง
- แสดง usage ของ agent subscriptions ทั้งหมด (เช่น Claude Code, Codex) ในแอปเดียว
- ทั้ง Moshi และ Termius สามารถใช้ร่วมกันได้ ไม่ใช่ตัวเลือกแบบ either-or
- ความประทับใจแรก: แอปขัดเกลา ลื่นไหล ตอบสนองดี แม้จะเป็นแอปใหม่พอสมควร

## ความเห็นสรุป

Moshi เป็นแอปที่น่าสนใจมากสำหรับใครที่รัน AI coding agents บนเครื่องของตัวเองแล้วอยากควบคุมจากมือถือ โดยเฉพาะเมื่อใช้ร่วมกับ Herder บนเครื่องที่เปิดทิ้งไว้ตลอดเช่น Spark ฟังก์ชัน agent inbox, hooks และ live activity บนหน้าจอล็อกทำให้การอนุมัติและติดตาม agents สะดวกมาก แม้จะเป็นแอปใหม่แต่ดูขัดเกลาและมีศักยภาพสูง

เสียงพากย์ไทย: ![[o1Zfr4CMt-U.mp3]]
