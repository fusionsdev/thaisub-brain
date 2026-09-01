---
videoId: "JgkD-PZ9bAo"
title: "Buzz Beginner's Guide: An Open Source, Agent-First Slack?"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=JgkD-PZ9bAo"
published: "2026-07-29"
has_voiceover: true
status: translated
synced_at: "2026-09-02"
tags: [thai-sub, youtube]
---

# Buzz Beginner's Guide: An Open Source, Agent-First Slack?

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=JgkD-PZ9bAo

## 📝 สรุป

# สรุป: Buzz Beginner's Guide: An Open Source, Agent-First Slack?

- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~19 นาที · **ลิงก์:** https://www.youtube.com/watch?v=JgkD-PZ9bAo

## ประเด็นหลัก

- **Buzz คือแอปแชตโอเพนซอร์ส** จาก Block ที่นำแนวคิด "agent-first" มาใช้ — โดย AI agent เป็นสมาชิกของห้องแชตจริงๆ ไม่ใช่บอทที่เสียบเข้ามา
- **สถาปัตยกรรมหลัก:** หนึ่งคอมมูนิตี้ หนึ่งโมเดลตัวตน หนึ่ง event log — ทุกสิ่ง (ข้อความ, รีแอกชัน, workflow, การอนุมัติ, Git push) เป็น signed event ใน append-only log ตัวเดียวกัน
- **ตั้งอยู่บนโปรโตคอล Nostr** — โปรโตคอลเปิดสำหรับข้อความที่ลงนามแล้ว ตัวตนคือ key pair ไม่ต้องสมัคร ไม่ต้องมีรหัสผ่าน ไม่ใช่ blockchain แต่มีความเป็นไปได้ในอนาคตที่จะเชื่อมต่อกับ Bitcoin
- **ความแตกต่างจากแชตบอททั่วไป:** Buzz agent มี key pair เป็นของตัวเอง มีสมาชิกภาพในช่องเฉพาะ และมีบันทึกการลงนามใน log เดียวกันกับมนุษย์ — ถือเป็น first-class citizen
- **ฟีเจอร์ที่พร้อมใช้งาน:** relay, channels, threads, DMs, canvases, แอปเดสก์ท็อป, Buzz CLI
- **รองรับหลาย agent runtime:** Claude Code, Codex, Goose, Buzz agent — ผู้ใช้สามารถตั้งค่า default และปรับแต่ง provider ได้
- **ระบบความจำของ agent (memories):** agent สามารถจดจำข้อมูลผู้ใช้ได้ (เช่น ชื่อ, ช่อง YouTube) ผ่าน core memory system
- **Workspace เฉพาะของ agent:** แต่ละ agent มีไดเรกทอรีถาวรเป็นของตัวเอง (.buzz) เก็บ research, plans, guides, work logs, repos, models — ทั้งหมดอยู่ในเครื่องของคุณ ไม่ใช่คลาวด์
- **Buzz shared compute:** ฟีเจอร์แชร์พลังการประมวลผลและโมเดลภายในเครื่องกับสมาชิกในกลุ่ม (ต้องใช้ Linux สำหรับฟีเจอร์ mesh)
- **การสร้างคอมมูนิตี้และกลุ่ม:** สามารถสร้างได้ง่าย ตั้งค่าเป็นส่วนตัวหรือสาธารณะ สร้าง agent team เพื่อเพิ่ม agent หลายตัวเข้า channel พร้อมกัน
- **แอปมือถือ:** มีแอปมือถือแล้ว เชื่อมต่อผ่าน QR code มีฟีเจอร์ครบเหมือนเดสก์ท็อป
- **ยังอยู่ในช่วงเริ่มต้น** แต่ศักยภาพและวิสัยทัศน์น่าประทับใจ — อาจมีการพัฒนาต่อไปในอนาคต

## ความเห็นสรุป

Buzz เป็นโปรเจกต์ที่น่าสนใจมากในแง่ของวิสัยทัศน์ — การทำให้ AI agent เป็นสมาชิกแรงก์เทียบมนุษย์ในแพลตฟอร์มแชต โดยใช้สถาปัตยกรรม Nostr ที่ตรวจสอบได้และกระจายศูนย์ แม้ยังเป็นช่วงเริ่มต้นและฟีเจอร์บางอย่างยังจำกัด (เช่น shared compute บน Windows) แต่แนวคิดการแชร์พลังการประมวลผลและโมเดลระหว่างสมาชิกในกลุ่มเป็นสิ่งที่มีศักยภาพสูง คุ้มค่าที่จะติดตามต่อไปครับ

เสียงพากย์ไทย: ![[JgkD-PZ9bAo.mp3]]
