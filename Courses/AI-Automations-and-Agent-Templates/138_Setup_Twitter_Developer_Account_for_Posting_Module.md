---
course: "AI Automations & Agent Templates"
lesson: "138 Setup Twitter Developer Account for Posting Module"
has_voiceover: false
has_subtitles: true
status: translated
synced_at: "2026-08-09"
tags: [thai-sub, course, ai_automations_and_agent_templates]
---

# 138 Setup Twitter Developer Account for Posting Module

## 📝 คำแปล

# 138_Setup_Twitter_Developer_Account_for_Posting_Module

- **วิดีโอต้นฉบับ:** local:138_Setup_Twitter_Developer_Account_for_Posting_Module
- **ช่อง:** AI Automations and Agent Templates
- **ความยาว:** ~2 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)

---

## บทนำ
วิดีโอนี้เป็นขั้นตอนการตั้งค่าบัญชี Twitter Developer เพื่อใช้กับโมดูลโพสต์ของระบบออโตเมชัน โดยเริ่มจากการสร้างแอปบน developer.x.com ตั้งค่าการยืนยันตัวตนผู้ใช้ รับ API key และ secret จากนั้นนำไปเชื่อมต่อกับโมดูล Twitter ในระบบ

## คำแปลเต็ม
เข้าไปที่ developer.x.com แล้วล็อกอินเข้าบัญชีของคุณ จากนั้นไปที่ developer portal คุณต้องสร้างแอป (create an app) ผมจะใช้ชื่อเดียวกันเลย ใส่ชื่อลงตรงนี้แล้วคลิก "Next" ต่อไปไปที่ "App Settings" เราต้องตั้งค่า user authentication settings ตรงนี้คุณต้องเลือกอันล่างสุดคือ read and write และ direct message จากนั้นไปที่ web app เราต้องเพิ่ม URLs ซึ่งคุณจะหาได้จากแหล่งข้อมูล (resource) ด้านล่างวิดีโอนี้

ตรงนี้เราต้องเพิ่ม URL สองอัน อันแรกก่อน จากนั้นคลิก "add another one" แล้วเพิ่มอันที่สองไว้ข้างล่าง จากนั้นก็เพิ่มอันนี้ สำหรับ terms of service เราก็ใส่สองอันนี้ คลิก "save" ตอนนี้เราสามารถไปที่ "keys and Tokens" แล้วไปที่ "API key and secret" คลิกตรงนี้ แล้วคัดลอกกลับไป ใส่ API key และใส่ API secret คลิก จากนั้นระบบจะให้คุณล็อกอินเข้าบัญชี Twitter คลิก "Authorize" และเมื่อการอนุญาตเสร็จสิ้น คุณก็ไปยังขั้นตอนถัดไปได้

เราต้องเพิ่มโมดูล Twitter อีกอันหนึ่ง ซึ่งเลือกได้ตรงนี้เท่านั้น เราไปที่ "6" และตรงนี้ไปที่ "create a post" คุณต้องเพิ่มข้อมูลอีกชุดหนึ่งที่เรียกว่า client ID และ client secret ดังนั้นกลับไปที่ developer portal แล้วคุณจะพบข้อมูลเหล่านี้ตรงนี้ ไปที่ "regenerate" แล้วเราจะได้ client secret วางลงตรงนี้ และตรงนี้คือ client ID คลิก "save" แล้วระบบจะให้เราอนุญาตแอป (authorize app) จากนั้นคุณก็สามารถโพสต์ลงบัญชีของคุณได้

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — เข้าไปที่ developer.x.com แล้วล็อกอินเข้าบัญชีของคุณ

**00:00:05** — จากนั้นไปที่ developer portal คุณต้องสร้างแอป (create

**00:00:11** — an app) ผมจะใช้ชื่อเดียวกันเลย ใส่ชื่อลงตรงนี้แล้วคลิก

**00:00:16** — "Next" ต่อไปไปที่ "App Settings" เราต้องตั้งค่า

**00:00:21** — user authentication settings ตรงนี้คุณต้องเลือกอันล่างสุดคือ

**00:00:28** — read and write และ direct message จากนั้นไปที่ web

**00:00:33** — app เราต้องเพิ่ม URLs ซึ่งคุณจะหาได้จากแหล่งข้อมูล

**00:00:38** — (resource) ด้านล่างวิดีโอนี้ ตรงนี้เราต้องเพิ่ม

**00:00:43** — URL สองอัน อันแรกก่อน จากนั้นคลิก "add another one"

**00:00:49** — แล้วเพิ่มอันที่สองไว้ข้างล่าง จากนั้นก็เพิ่มอันนี้

**00:00:54** — สำหรับ terms of service เราก็ใส่สองอันนี้ คลิก "save"

**00:00:59** — ตอนนี้เราสามารถไปที่ "keys and Tokens" แล้วไปที่

**00:01:04** — "API key and secret" คลิกตรงนี้ แล้วคัดลอกกลับไป

**00:01:10** — ใส่ API key และใส่ API secret คลิก จากนั้นระบบจะให้คุณล็อกอินเข้าบัญชี

**00:01:17** — Twitter คลิก "Authorize" และเมื่อการอนุญาตเสร็จสิ้น

**00:01:22** — คุณก็ไปยังขั้นตอนถัดไปได้ เราต้องเพิ่มโมดูล Twitter

**00:01:28** — อีกอันหนึ่ง ซึ่งเลือกได้ตรงนี้เท่านั้น เราไปที่

**00:01:33** — "6" และตรงนี้ไปที่ "create a post" คุณต้องเพิ่มข้อมูลอีกชุดหนึ่งที่เรียกว่า

**00:01:41** — client ID และ client secret ดังนั้นกลับไปที่ developer

**00:01:46** — portal แล้วคุณจะพบข้อมูลเหล่านี้ตรงนี้ ไปที่ "regenerate"

**00:01:52** — แล้วเราจะได้ client secret วางลงตรงนี้ และตรงนี้คือ

**00:01:58** — client ID คลิก "save" แล้วระบบจะให้เราอนุญาตแอป

**00:02:03** — (authorize app) จากนั้นคุณก็สามารถโพสต์ลงบัญชีของคุณได้

