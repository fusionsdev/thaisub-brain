---
videoId: "mnBQTECjvKc"
title: "Hermes Desktop Masterclass: 1. Installation, UI, Settings & Backends"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=mnBQTECjvKc"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-08"
tags: [thai-sub, youtube]
---

# Hermes Desktop Masterclass: 1. Installation, UI, Settings & Backends

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=mnBQTECjvKc

## 📝 สรุป

# สรุปภาษาไทย — Hermes Desktop Masterclass: 1. Installation, UI, Settings & Backends

> **ที่มา:** [YouTube — Tonbi's AI Garage](https://www.youtube.com/watch?v=mnBQTECjvKc) · เผยแพร่ 4 ก.ย. 2026 · ~34:36 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Tonbi's AI Garage*

## วิดีโอนี้เกี่ยวกับอะไร
โมดูลที่หนึ่งของซีรีส์มาสเตอร์คลาสแอป **Hermes Desktop** (3 โมดูล) ว่าด้วยเรื่องพื้นฐานทั้งหมด ได้แก่ แนวคิดว่าแอปคืออะไร วิธีติดตั้ง ทัวร์ส่วนติดต่อผู้ใช้ หน้าตั้งค่าทุกหน้า และวิธีเชื่อมต่อกับ backend หลายแบบ ทั้งเครื่อง local, Hermes Cloud, remote gateway และ SSH

## ประเด็นหลัก

1. **ภาพจำที่ถูกต้อง:** แอปคือ frontend ส่วนเอเจนต์รันอยู่บน backend ที่ชื่อ **Hermes Serve** (เซิร์ฟเวอร์ JSON RPC websocket แบบ headless ที่แอปสร้างและดูแลเอง) เปิดแอปบนเครื่องที่มี Hermes Agent อยู่แล้วจะได้ session, ความจำ, skill และ config เดิมจาก TUI ทันที
2. **ติดตั้ง:** โหลดตามระบบปฏิบัติการจากเว็บ Nous Research หรือสั่ง `hermes-desktop` จากเทอร์มินัล มีแล้วลงแค่ส่วนหน้า ยังไม่มีก็ลงเอเจนต์ให้ด้วย ติดตั้งผ่าน pip และ Homebrew ไม่รองรับแล้ว มี flag อย่างกำหนด working directory, `skip build` และ `force build`
3. **ทัวร์ UI:** แถบซ้ายมี new session, แท็บ capabilities (skills / tools / MCP พร้อม skills hub และ catalog), messaging (Telegram, WhatsApp และอื่น), artifacts, scheduled jobs (ชื่อใหม่ของ cron job พร้อม blueprint), pinned session, รายชื่อ session และโปรไฟล์ แถบล่างคือ status bar (command center, ตัวสลับ backend, gateway, อัปเดต ปรับแต่งได้ กด `Ctrl K` ค้นหาทุกคำสั่ง กด `control shift S` เปิดปิด status bar)
4. **ตั้งค่า:** หน้า model (โมเดลเริ่มต้นรายโปรไฟล์, provider, reasoning, fast mode, auxiliary model อย่าง vision, compression, approvals, MCP, title gen และ review ผ่านคำสั่ง `/review`), chat (personality, time zone, reasoning blocks, image attachments), appearance (ธีม mono, Cyber Punk และอื่น), workspace, safety (approval mode แนะนำ smart), browser (ใช้ real browser profile ทั้ง Chrome, Brave, Edge), memory and context, voice, advanced, notifications, billing ของ Nous Portal (โมเดลกว่า 200 ตัว), providers กับ API key, gateways, keyboard shortcuts, tools and keys, plugins และ archive chats
5. **Backend:** local gateway คือเครื่องปัจจุบัน ส่วนแบบอื่นทำผ่าน gateways ได้แก่ **Hermes Cloud** (สร้าง agent ใน Nous Portal แล้วลงชื่อเข้าผ่าน Gmail กดเชื่อมทีเดียว), **remote gateway** (รัน `hermes serve` ระบุ host กับ port แล้วกรอก IP กับ port ที่อีกเครื่องพร้อม username กับ password) และ **SSH** (ตัวที่ผู้สร้างแนะนำ เปิด SSH อนุญาตผ่าน `sudo ufw allow ssh` หา IP จาก `ip route get` ใส่กุญแจผ่าน `ssh-keygen` แล้วเพิ่มใน gateway) สลับ backend ได้คลิกเดียว อัปเดตทุก instance ได้ทีเดียว token เก็บเป็นไฟล์เฉพาะเจ้าของที่ main process ถือ UI กับปลั๊กอินไม่เห็น token โดยตรง
6. **โมดูลต่อไป:** โมดูลสองคือลงมือทำงานจริง (session, project, composer, เสียง และ gig cockpit) โมดูลสามคือการปรับแต่ง (plugin, bot mode, HUD mode)

## ใครควรดู
ผู้ใช้ Hermes Agent ที่อยากย้ายงานหลักมาอยู่บนแอปเดสก์ท็อป และคนที่มีเอเจนต์หลายเครื่อง (PC, แล็ปท็อป, VPS, DGX Spark) แล้วอยากคุมทั้งหมดจากหน้าจอเดียว

---
*Attribution: Hermes Desktop Masterclass: 1. Installation, UI, Settings & Backends — Tonbi's AI Garage (youtube.com/watch?v=mnBQTECjvKc), เผยแพร่ 4 ก.ย. 2026*

เสียงพากย์ไทย: ![[mnBQTECjvKc.mp3]]

