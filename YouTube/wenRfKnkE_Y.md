---
videoId: "wenRfKnkE_Y"
title: "Exploring Hermes Plugins: REA and Meshy"
channel: "Tonbi's AI Garage"
url: "https://www.youtube.com/watch?v=wenRfKnkE_Y"
published: ""
has_voiceover: true
status: translated
synced_at: "2026-10-24"
tags: [thai-sub, youtube]
---

# Exploring Hermes Plugins: REA and Meshy

> [!info] แหล่งที่มา
> Tonbi's AI Garage · https://www.youtube.com/watch?v=wenRfKnkE_Y

## 📝 สรุป

# สรุปภาษาไทย — Exploring Hermes Plugins: REA and Meshy

> **ที่มา:** [YouTube — Tonbi's AI Garage](https://www.youtube.com/watch?v=wenRfKnkE_Y) · เผยแพร่ 23 ต.ค. 2026 · ~17:14 นาที
> *สรุปโดยอัตโนมัติ — เนื้อหาต้นฉบับ © Tonbi's AI Garage*

## วิดีโอนี้เกี่ยวกับอะไร
เดโมปลั๊กอินทางการสองตัวของ Hermes Agent ที่ทำงานผ่านเซิร์ฟเวอร์ MCP ได้แก่ **REA** เครื่องมือช่วยรีเวิร์สเอนจิเนียร์ซอฟต์แวร์ และ **Meshy** แอปสร้างโมเดล 3 มิติสำหรับเกม พร้อมวิธีติดตั้ง ตั้งค่า และตัวอย่างใช้งานจริง

## ประเด็นหลัก

1. **ภาพรวม:** Hermes Agent กำลังผลักดันปลั๊กอินทั้งทางการและจากชุมชนใน plugins catalog วิดีโอนี้หยิบสองตัวฮิตมาโชว์คือ REA กับ Meshy (เดโมเคยลงบน X มาก่อน แต่มีฟุตเทจทดสอบ Meshy เพิ่มใหม่)
2. **REA คืออะไร:** รีโปโอเพนซอร์ส Reverse Engineer Anything สำหรับเรียนรู้วิธีรีเวิร์สเอนจิเนียร์แอปด้วยโค้ดดิ้งเอเจนต์ ปลั๊กอินทางการประกอบด้วยไฟล์ตั้งค่า MCP (MCP.json ต่อเซิร์ฟเวอร์ REA MCP) กับไฟล์สกิล (skill MD) ที่สอนเอเจนต์วิธีใช้รีโป
3. **ติดตั้ง REA:** คำสั่ง `Hermes plugin install REA` ดูแลโดย Nous Research เอง ตรวจว่าเปิดใช้แล้วด้วย `slash plugins` แล้วถามเอเจนต์ว่าปลั๊กอินมีอะไรและใช้อย่างไร
4. **REA ทำอะไร:** วิเคราะห์ซอฟต์แวร์ที่ build แล้ว คืนผลแบบมีโครงสร้าง แต่ละผลมี evidence ID ให้เอเจนต์อ้างอิง เซิร์ฟเวอร์มีเครื่องมือราว 170 ตัว ทดสอบเรียกเครื่องมือแล้วทำงานได้
5. **ลองกับแอปจริง:** เอา REA วิเคราะห์ Garage Studio แอปบันทึกวิดีโอที่ผู้สร้างเขียนเองบนพื้นฐานโปรเจกต์โอเพนซอร์ส Recordly (เคยใช้ REA ถอดโค้ดแอปตัดต่อตัวอื่นหามุกปรับปรุงมาก่อน เต็มๆ จะลงเป็นวิดีโอแยกวันจันทร์หน้า) ผลคือแจกแจงวินโดว์ 6 อัน web security preload API IPC และเครือข่าย เอเจนต์เอาไปต่อยอดสร้างใหม่ได้ เป็นเครื่องมือเชิงสืบสวนมากกว่าช่างซ่อมโดยตรง
6. **ดีล Meshy:** Nous Research จับมือ Meshy ให้ผู้ใช้ Hermes ใช้แพ็กเกจ pro 1 เดือนเพียง 1 ดอลลาร์ (ปกติ 20 ดอลลาร์) ดีลจำกัดเวลา Meshy AI คือสายสร้างโมเดล 3 มิติสำหรับเกมและสภาพแวดล้อม
7. **ติดตั้ง Meshy:** ต้องมีบัญชี meshy.ai อย่างน้อยระดับ pro เพราะปลั๊กอินต้องใช้ API กด add ในแค็ตตาล็อก (ต้องใช้ Hermes Agent เวอร์ชันล่าสุด) แล้วเอาคีย์จาก meshy.ai/developers หัวข้อ MCP มาวางที่ settings > plugins มีตัวเลือก inline 3D cards in chat credit balance และ status bar
8. **ทดสอบครั้งแรก:** ถาม `can you test the Meshy plugin?` เอเจนต์รันเช็ก read-only ผ่านหมด คีย์ใช้ได้ แล้วลองของเล็กคือหีบสมบัติไม้ 5 เครดิต มีระบบ approval ก่อนใช้เงิน ผู้สร้างตั้ง spend limit แชทนี้ไว้ 200 เครดิต
9. **ของที่ได้จากหีบ:** มีแถบ Meshy 2% previewing เครดิตลด 5 ได้พรีวิวมาดูแบบ 3 มิติหมุนได้ในแอป มี wireframe auto rotate grid ดูโฟลเดอร์ได้ การ์ดโชว์เครดิตตลอด แล้วกด texture แบบ realistic ได้ใน 2-3 นาที มี remesh regenerate ดาวน์โหลดแปลงได้หลายฟอร์แมต เอาไปเป็น in-game asset ได้เลย
10. **ของยากขึ้น (Yeti):** Meshy มีตัวสร้างภาพในตัวใช้ GBT images หรือจะสร้างภาพใน Hermes ก่อนก็ได้ (ถ้าไม่มีบัญชี codex) เอาภาพอสูร Yeti 2 มิติมาแปลงเป็น 3 มิติ เลือก smart topography clean mesh ก่อน (อีกแบบคือ Meshy 7.1 full detail) แล้ว rig 5 เครดิตแถมแอนิเมชันเดินวิ่งฟรี ได้ทั้งตัวยืน เดิน วิ่ง เก็บในคลังแอสเซ็ตของปลั๊กอิน
11. **ของยากสุด (มังกรแดง):** สั่งสั้นๆ ว่า can we make a red dragon เอเจนต์ถามกลับเรื่องวิธีสร้าง (3 แบบมีพื้นผิวหมด) เลือก max detail 30 เครดิต ระบุใช้ในเกม (เกี่ยวกับ triangle count) สไตล์ realistic and fearsome ได้มังกรน่ากลัวจากพรอมต์เดียว มีหางแฉกแปลกๆ (double tail) ต้อง refine ต่อ ส่วน rigging ใช้ได้เฉพาะตัวละครคล้ายมนุษย์ มังกรเลยอด

## บทสรุป
สองปลั๊กอินเสริมเอเจนต์คนละทาง REA สายวิเคราะห์เจาะซอฟต์แวร์ Meshy สายสร้างแอสเซ็ต 3 มิติไวใช้ในเกม ทั้งคู่ติดตั้งง่ายผ่านแค็ตตาล็อกทางการ ผู้สร้างชวนคอมเมนต์ว่าแต่ละคนกำลังสร้างอะไรด้วยปลั๊กอินไหน และจะทยอยลองปลั๊กอินตัวอื่นๆ ต่อ

## ใครควรดู
คนใช้ Hermes Agent คนทำเกมที่อยากได้แอสเซ็ต 3 มิติไวๆ และคนที่สนใจเอาปลั๊กอิน MCP มาต่อเอเจนต์ให้เก่งขึ้น

---
*Attribution: Exploring Hermes Plugins: REA and Meshy — Tonbi's AI Garage (youtube.com/watch?v=wenRfKnkE_Y), เผยแพร่ 23 ต.ค. 2026*

เสียงพากย์ไทย: ![[wenRfKnkE_Y.mp3]]

