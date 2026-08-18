---
videoId: "SLUtt-po_OE"
title: "The Ultimate Guide to Hermes Desktop Plugins"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=SLUtt-po_OE"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-08-19"
tags: [thai-sub, youtube]
---

# The Ultimate Guide to Hermes Desktop Plugins

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=SLUtt-po_OE

## 📝 สรุป

# สรุป: The Ultimate Guide to Hermes Desktop Plugins
- **ช่อง:** Tonbi's AI Garage · **ความยาว:** ~20 นาที · **ลิงก์:** https://www.youtube.com/watch?v=SLUtt-po_OE
## ประเด็นหลัก
- Hermes Desktop Plugin SDK ช่วยให้สร้าง plugin (ปลั๊กอิน/ส่วนขยาย) ใส่ลงในแอป Hermes Agent Desktop ได้ โดยผู้สร้างพบตำแหน่งวาง plugin ทั้งหมด 25 จุดในแอป
- ตำแหน่งวางมีตั้งแต่ pane (แผงหน้าต่าง) ทั้ง 4 ทิศ, workspace แบบ docked, status bar, title bar, popover ทั้ง 4 ทิศ, จุดต่างๆ รอบ composer ไปจนถึง route และ sidebar — แต่ละตำแหน่งเหมาะกับรูปแบบ UI ที่ต่างกัน
- หลักการออกแบบคือ form follows the job: compact สำหรับข้อมูลสถานะแบบพื้นหลัง, anchored สำหรับการควบคุมเร็ว, expansive สำหรับแอปเต็มรูปแบบ และ declarative สำหรับ UI ที่ Hermes เป็นเจ้าของ
- แหล่งพลังของ plugin มาจากสถานะของ Hermes เอง, การใช้ Hermes เป็น gateway (ข้อมูล sessions, cron jobs, Kanban), การต่อ backend ภายนอก และการเรนเดอร์ media ผ่านเบราว์เซอร์
- ข้อจำกัดที่ต้องรู้: plugin เข้าถึง native API หรือโหนดตามอำเภอใจไม่ได้, ใช้ได้เฉพาะพื้นที่ที่ Hermes จัดสรรให้, พื้นที่เก็บเป็นแค่ JSON เล็กๆ, ไม่รันเมื่อปิดแอป และไม่ใช่เลเยอร์สำหรับระบบเนทีฟที่ต้องสิทธิพิเศษ
- สถาปัตยกรรมแนะนำ: plugin เป็น UI เชื่อมต่อ backend ซึ่งเชื่อมต่อบริการเฉพาะทาง เช่น การต่อ Hermes กับบริการ FFmpeg สำหรับตัดต่อวิดีโอ
- สาธิตการสร้างเทรดดิ้งเทอร์มินัลจริง: ปลั๊กอิน Hyperliquid แบบ read-only บน sidebar มี watch list, order book, ราคาปัจจุบัน และกราฟ TradingView เต็มรูปแบบ
- สาธิต plugin Spotify แบบ popover: ค้นหาศิลปินและควบคุมเพลงในแอปได้ แต่ต้องเปิดแอป Spotify บนเดสก์ท็อปไว้ (ทำหน้าที่เป็นตัวควบคุมมากกว่าเครื่องเล่น)
- สาธิต SNES emulator: เล่นเกมอย่าง Legend of Zelda: A Link to the Past ผ่าน emulator.js จากไฟล์ ROM หยุดพักกลางเกมแล้วกลับมาทำงานต่อได้
- ผู้สร้างวางแผนจะเปิดซอร์สปลั๊กอินทั้งหมดบน GitHub เมื่อเก็บรายละเอียดเรียบร้อย
## ความเห็นสรุป
วิดีโอนี้เหมาะสำหรับผู้ใช้ Hermes Agent Desktop ที่อยากต่อยอดจากแอปพื้นฐานไปสู่การสร้างเครื่องมือเฉพาะทางของตัวเอง เพราะได้ทั้งกรอบคิด (ว่าอะไรควรเป็น plugin อะไรไม่ควร) และตัวอย่างการใช้งานจริงที่ทำตามได้ พร้อมทั้งเปิดเผยข้อจำกัดของระบบอย่างตรงไปตรงมา จุดเด่นคือการสาธิตแบบเห็นจริงทุกตำแหน่งวาง ทำให้เห็นภาพชัดว่า UI แต่ละแบบเหมาะกับงานแบบไหน

เสียงพากย์ไทย: ![[SLUtt-po_OE.mp3]]

