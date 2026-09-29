---
videoId: "16QTif1cqoU"
title: "Day 4A: Multi-Agent Systems — Roles, Communication, Orchestration"
channel: "Adspolitan Knowledge Studio"
url: "https://www.youtube.com/watch?v=16QTif1cqoU"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-09-29"
tags: [thai-sub, youtube]
---

# Day 4A: Multi-Agent Systems — Roles, Communication, Orchestration

> [!info] แหล่งที่มา
> Adspolitan Knowledge Studio · https://www.youtube.com/watch?v=16QTif1cqoU

## 📝 สรุป

# สรุป: Day 4A: Multi-Agent Systems — Roles, Communication, Orchestration

- **ช่อง:** Adspolitan Knowledge Studio · **ความยาว:** ~24 นาที · **ลิงก์:** https://www.youtube.com/watch?v=16QTif1cqoU

## ประเด็นหลัก

- แม้ชื่อวิดีโอจะระบุ Multi-Agent Systems แต่เนื้อหาจริงของ assignment นี้คือ agent quality ที่มีรากฐานอยู่ที่ observability (การสังเกตการทำงานของเอเจนต์)
- เสาหลักของ agent observability มี 3 อย่าง: logs (เกิดอะไรขึ้นตอนไหน) traces (ทำไมผลลัพธ์จึงเป็นแบบนั้น — ลำดับขั้นตอนทั้งหมด) และ metrics (คะแนนว่าเอเจนต์ทำได้ดีแค่ไหน) — อธิบายด้วยอุปมาการทำอาหาร: logs = บันทึกวัตถุดิบ+ขั้นตอน, traces = ทำตามสูตรจริง, metrics = ให้คะแนนอาหาร
- ตัวอย่าง bug จริง: root agent ส่ง list ของ paper เป็น string แทน list ของ string ทำให้นับได้ 1690 paper แทนที่จะเป็น 14 — แก้ด้วยการตรวจ invocations ใน ADK web UI เห็น parameter ที่ LLM รับจริง
- การ debug ด้วย ADK web UI ใช้ได้ในช่วงพัฒนา แต่ production ไม่มีสิทธิ์เข้า web UI และเอเจนต์อาจรันวันละพันครั้ง — ต้องเก็บ observability data ด้วย log statements แทน
- Plugin คือโมดูลโค้ดที่รันอัตโนมัติตามช่วงต่างๆ ของวงจรเอเจนต์ ประกอบด้วย callbacks หลายตัว (before/after agent, before/after model, before/after tool, after error) — callbacks รวมกันเป็น plugin
- ตัวอย่าง CountInvocationPlugin นับจำนวนครั้งที่เอเจนต์และ LLM ถูกเรียก โดยเพิ่มค่าทีละหนึ่งใน before callback แต่ละตัว
- ไดอะแกรม 6 ขั้นตอนอธิบาย flow: user message → runner → plugin (before agent) → research agent → LLM (plugin ก่อน/หลัง model) → response กลับ — plugin ถูกเรียก 2 ครั้งต่อการรันหนึ่งครั้ง
- ADK มี built-in logging plugin ที่เก็บอัตโนมัติ: user messages, agent responses, timing data, LLM request/response, tool calls และ execution traces ทั้งหมด
- การใช้งาน: import plugin แล้วเสียบเข้าตอนสร้าง runner — log ที่ได้อ่านง่ายและอธิบายตัวเองได้ ไล่ดู invocation ID, event ID, token ได้ครบ
- วิดีโอถัดไป (Day 4B) คือ evaluation — การให้คะแนนคุณภาพคำตอบและการใช้ tool ของเอเจนต์

## ความเห็นสรุป

วิดีโอนี้เดินตาม notebook ทีละ cell เหมือนคลิปก่อนๆ ของซีรีส์ จุดเด่นคือการพา debug bug จริง (string แทน list) จนเห็นกันชัดๆ ว่า observability ช่วยหาสาเหตุได้อย่างไร แล้วต่อยอดสู่ logging แบบ plugin สำหรับ production ครับ ข้อควรระวังอีกอย่างคือชื่อวิดีโอกับเนื้อหาจริงไม่ตรงกันอีกครั้ง (ชื่อบอก Multi-Agent แต่สอน Observability/Logging) ผู้เรียนควรอาศัยคำอธิบายในวิดีโอเป็นหลักแทนชื่อคลิปครับ

เสียงพากย์ไทย: ![[16QTif1cqoU.mp3]]

