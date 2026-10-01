---
videoId: "_h3XJskyZuQ"
title: "Complete Guide to building a website with Claude (Step by Step)"
channel: "Ray Fu"
url: "https://www.youtube.com/watch?v=_h3XJskyZuQ"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-02"
tags: [thai-sub, youtube]
---

# Complete Guide to building a website with Claude (Step by Step)

> [!info] แหล่งที่มา
> Ray Fu · https://www.youtube.com/watch?v=_h3XJskyZuQ

## 📝 สรุป

# สรุป: Complete Guide to building a website with Claude (Step by Step)

- **ช่อง:** Ray Fu · **ความยาว:** ~12 นาที · **ลิงก์:** https://www.youtube.com/watch?v=_h3XJskyZuQ

## ประเด็นหลัก

- วิดีโอนี้คือเวอร์ชัน "สำหรับมือใหม่" จากคลิปก่อนหน้าที่ถูกบอกว่าเร็วเกินไป ทำเป็นซีรีส์สอนทีละขั้นตอน
- เริ่มจาก Claude Design (ต้องมี subscription แบบ Pro) สร้าง design system ซึ่งเปรียบเป็น "คลังความจำ" เก็บอัตลักษณ์แบรนด์ ทั้งสี ฟอนต์ โทนการสื่อสาร
- กรอกชื่อบริษัท คำอธิบาย สี และฟอนต์ แล้วกด generate — Claude จะไล่ทำงานเอง แล้วให้เรารีวิวทีละ item แบบ looks good / needs work
- บน Claude Design แก้ดีไซน์ได้ 3 ทาง: คลิกแก้ตรง ๆ แบบ Squarespace, ฝากคอมเมนต์, และใช้ฟังก์ชัน draw วนพื้นที่ที่ต้องการแก้
- ส่งต่องานด้วยปุ่ม hand off to Claude Code พร้อมสร้างโฟลเดอร์โปรเจกต์ + ไฟล์ .md ซึ่งทำหน้าที่เป็น "ความจำ" ของ Claude ให้ทำต่อได้แม้ปิดโปรเจกต์
- ติดตั้ง Node.js (เลือก LTS) แล้วให้ Claude Code แปลงเว็บ static เป็น Next.js แบบ full-stack
- ใช้ Supabase เป็น backend: สร้าง organization (แพ็กเกจฟรีก็เพียงพอ), new project, เปิด RLS, รันไฟล์ schema.sql ใน SQL editor สร้างตาราง แล้วเชื่อมผ่านไฟล์ .env.local ด้วย project URL + publishable key
- ตรวจเว็บด้วยคำสั่ง npm run dev แล้ว push ขึ้น GitHub (ถ้า URL repo ไม่ตรง ให้ถาม Claude ขอคำสั่งแก้)
- Deploy ด้วย Vercel: import repo, เพิ่ม environment variables ของ Supabase 2 ค่า แล้วกด deploy — เว็บออนไลน์บนโดเมน Vercel ทันที
- จดโดเมนเองทีหลังได้ แนะนำ GoDaddy หรือ Porkbun
- ของเพิ่มที่ยังไม่สอนในคลิป: ระบบอีเมล, PostHog/Vercel analytics, Google SEO

## ความเห็นสรุป

คลิปนี้เหมาะมากสำหรับผู้เริ่มต้นที่อยากได้เว็บ full-stack จริงจังโดยไม่ต้องเขียนโค้ดเอง เพราะอธิบายช้า ครบทุกคลิก และแก้ปัญหาที่เจอจริงระหว่างทำ (จอดำ, push ผิด repo) ให้ดูด้วย จุดที่ต้องระวังคือค่าใช้จ่าย subscription ของ Claude และการเก็บ secret key ให้ปลอดภัย

เสียงพากย์ไทย: ![[_h3XJskyZuQ.mp3]]

