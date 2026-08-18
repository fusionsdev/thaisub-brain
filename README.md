# ThaiSub Brain 🧠

คลังโน้ตสรุปวิดีโอแปลไทย — ทุกคลิป YouTube และบทเรียนคอร์สที่แปลโดย [thaisub.vercel.app](https://thaisub.vercel.app) pipeline

## โครงสร้าง

```
ThaiSub Brain/
├── YouTube/<videoId>.md        ← โน้ตวิดีโอเดี่ยว (169+ คลิป)
│   └── attachments/*.mp3       ← เสียงพากย์ไทย
├── Courses/<course>/           ← โน้ตบทเรียนแยกตามคอร์ส
│   ├── _index.md               ← สถานะ + wikilinks ทุกบท
│   └── attachments/*.mp3
├── Index/ · Templates/
└── ThaiSub Brain.md            ← Dashboard
```

## โน้ตแต่ละใบมีอะไร

- **Frontmatter** — `videoId`, `channel`, `url`, `has_voiceover`, `tags`
- **📝 สรุป** — สรุปภาษาไทยเต็มจาก pipeline แปล
- **📝 คำแปล / ⏱️ ซับไตเติ้ล** (โน้ตคอร์ส) — คำแปลเต็ม + ทุกประโยคพร้อม timestamp
- **เสียงพากย์ไทย** — embed `![[<id>.mp3]]` เล่นในโน้ตได้ (Obsidian/Tolaria)

## อัพเดทอัตโนมัติ

Pipeline (Hermes Agent cron) sync โน้ตใหม่ทุก 4 ชั่วโมง + หลังจบรอบแปล แล้ว push ขึ้น repo นี้

## เครื่องมือที่ใช้อ่าน

ทำงานกับทั้ง **Tolaria** (preferred — MCP + git sync ในตัว) และ **Obsidian** — เป็น plain Markdown ธรรมดา

## License / Attribution

โน้ตเป็นสรุป/คำแปลเพื่อการอ่านส่วนตัว — สิทธิ์วิดีโอต้นฉบับเป็นของเจ้าของช่องแต่ละราย (ดูลิงก์แหล่งที่มาในแต่ละโน้ต)
