---
videoId: "Ex-eGzpS53s"
title: "OpenWork: One MCP Hub for Every AI Agent — Install, Self-Host & Supercharge Your Workflow"
channel: "Full Stack"
url: "https://www.youtube.com/watch?v=Ex-eGzpS53s"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# OpenWork: One MCP Hub for Every AI Agent — Install, Self-Host & Supercharge Your Workflow

> [!info] แหล่งที่มา
> Full Stack · https://www.youtube.com/watch?v=Ex-eGzpS53s

## 📝 สรุป

# สรุป: OpenWork: One MCP Hub for Every AI Agent — Install, Self-Host & Supercharge Your Workflow
- **ช่อง:** Full Stack · **ความยาว:** ~12 นาที · **ลิงก์:** https://www.youtube.com/watch?v=Ex-eGzpS53s

## ประเด็นหลัก
- ปัญหาหลัก: สกิล พรอมป์ และบริการของเอเจนต์ AI ติดอยู่ภายในเครื่องมือแต่ละตัว (Claude Code, Cursor, Codex) ไม่สามารถแชร์หรือพกพาข้ามเครื่องมือได้ และทีมก็ไม่มีแหล่งความจริงร่วมกัน
- OpenWork คือแอปเดสก์ท็อปโอเพนซอร์สฟรี ทางเลือกของ Claude Cowork และ Codex ขับเคลื่อนด้วย Open Code รองรับ macOS, Windows, Linux — เพิ่ม MCP ตัวเดียวก็ใช้สกิลและบริการชุดเดียวกันได้ทุกเอเจนต์
- กลไกหลักคือ OpenWork Connect: MCP server ตัวเดียว (ทั้ง local และ OpenWork Cloud) ที่เผยให้เห็นเครื่องมือสองอย่างคือ search capabilities (ค้นหา) และ execute capability (เรียกใช้)
- การติดตั้งเป็นพรอมป์ภาษาเดียวในเอเจนต์ เช่น `codex mcp add openwork` หรือ `claude mcp add` แบบ HTTP transport หรือคอนฟิก JSON ใน Open Code — ไม่มี vendor lock-in
- Self-host ได้ทั้งสแตก: API server, web dashboard, ฐานข้อมูล MySQL แอปเดสก์ท็อปเป็นแค่ไคลเอนต์ของ API
- แอปเดสก์ท็อปมี Artifacts, built-in browser control, การจัดการเซสชันแบบมี scopes/สิทธิ์/กู้คืนข้อผิดพลาด และ memory bank ที่มนุษย์ตรวจสอบก่อนบันทึก
- สำหรับองค์กร: OpenWork Den คือ control plane จัดการผู้ใช้ โมเดล นโยบายเดสก์ท็อป และมาร์เก็ตเพลส (เผยแพร่สกิล/ปลั๊กอิน) จากแดชบอร์ดเดียว พร้อม SCIM/SSO ผ่าน Microsoft Entra
- เทคนิค: PNPM monorepo + TurboRepo, Electron/React/TypeScript, Tailwind/Shadcn UI, TanStack Query, Zustand, Zod, Drizzle, Better Auth, MCP authorization + OAuth 2.1/PKCE
- การรองรับองค์กร: AWS EKS, Azure AKS, Google GKE + Helm charts, เซ็ตอัป air-gapped, Docker Compose
- ราคา: เริ่มฟรี (desktop app), Team Starter $50/เดือน (5 ที่นั่ง + API), Enterprise เพิ่ม SSO/SCIM
- สถานะ: เปิดตัวมกราคม 2026, ทะลุ 19,800 stars และดาวน์โหลดรวม 1.3 ล้านครั้งใน ~7 เดือน

## ความเห็นสรุป
วิดีโอนี้เป็นบทแนะนำที่ครอบคลุมและกระชับ เหมาะกับทั้งผู้ใช้รายบุคคลที่อยากรวมศูนย์เวิร์กโฟลว์ AI ของตัวเอง และทีม/องค์กรที่ต้องการ control plane สำหรับจัดการโมเดล สกิล และนโยบายแบบรวมศูนย์ จุดแข็งคือการอธิบายกลไก MCP ให้เข้าใจง่ายพร้อมตัวอย่างคำสั่งติดตั้งจริง แต่ข้อมูลบางส่วน (เช่น ยอดดาวน์โหลดและฟีเจอร์) เป็นข้อมูล ณ ช่วงที่อัดวิดีโอ ควรตรวจสอบกับเว็บไซต์ openworklabs.com ก่อนตัดสินใจใช้งานจริง

เสียงพากย์ไทย: ![[Ex-eGzpS53s.mp3]]

