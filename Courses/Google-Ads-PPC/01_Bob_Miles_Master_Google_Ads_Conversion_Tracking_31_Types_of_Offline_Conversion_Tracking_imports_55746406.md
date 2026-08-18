---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 31 Types of Offline Conversion Tracking imports 55746406"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 31 Types of Offline Conversion Tracking imports 55746406

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_31_Types_of_Offline_Conversion_Tracking_imports_55746406.mp3]]

## 📝 คำแปล

# Master Google Ads Conversion Tracking – ประเภทของการ Import Conversion แบบ Offline (Offline Conversion Tracking Imports)

- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_31_Types_of_Offline_Conversion_Tracking_imports_55746406 (วิดีโอท้องถิ่นในคอร์ส Google Ads PPC PayPerCall)
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~5 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)

---

## บทนำ

คลิปนี้ของ Bob Miles อธิบายวิธีการตั้งค่า offline conversion tracking (OCT) ทุกแบบที่มีใน Google Ads เริ่มจากวิธี native แบบ Conversions from clicks โดยใช้ Google Click ID (GCLID) และแบบ Enhanced Conversions for Leads รวมถึงการ import เข้า Salesforce และ HubSpot โดยตรง และวิธีผ่าน Zapier โดยสรุปว่าวิธี GCLID ให้ความแม่นยำสูงกว่า ในขณะที่ Enhanced Conversions for Leads ติดตั้งง่ายที่สุด

## คำแปลเต็ม

คุณสามารถตั้งค่า offline conversion tracking (การติดตามคอนเวอร์ชันนอกเว็บไซต์) ได้หลายวิธี และในคลิปนี้ผมจะบอกคุณถึงวิธีการติดตั้งทั้งหมดที่มีสำหรับ OCT และจะบอกว่าเมื่อไหร่ควรใช้วิธีไหน เริ่มจากประเภทของ offline conversion imports กันก่อน

อย่างแรก เรามีฟังก์ชัน native ที่สร้างไว้ใน Google Ads สำหรับการ import conversion ถ้าคุณเลือกวิธีนี้ โดยพื้นฐานคุณจะมีวิธีการติดตั้งหลักสองแบบ คุณสามารถเลือกแบบ Conversions from clicks โดยใช้ Google Click ID หรือที่รู้จักกันในชื่อ GCLID หรือคุณสามารถเลือกแบบ enhanced conversions for leads วิธีการทั้งสองทำงานต่างกัน และผมจะบอกความแตกต่างในสไลด์สองถัดไป

จากนั้นเรามี Google Ads Conversion Import แบบ built-in สำหรับ Salesforce และ HubSpot ถ้าคุณใช้หนึ่งในสองเครื่องมือยอดนิยมเหล่านี้ที่ใช้กันแพร่หลาย คุณสามารถซิงค์การ import conversion tracking ของคุณกับแพลตฟอร์ม CRM เหล่านี้ได้โดยตรง และยังมีวิธี offline conversion tracking ผ่าน Zapier ที่คุณสามารถเชื่อมต่อแอปทุกตัวเท่าที่มนุษย์รู้จักกับ Google ได้ แต่คุณต้องสร้าง Zap ภายใน Zapier เพื่อให้มันทำงาน

ผมชอบใช้วิธี native ดังนั้นผมจะเลือกแบบ Conversions from clicks โดยใช้ Google Click ID หรือแบบ enhanced conversions for leads วิธี enhanced conversions for leads นั้นติดตั้งง่ายที่สุด และนี่คือถ้าคุณได้ติดตั้ง enhanced conversions ไว้แล้ว ซึ่งเราได้พูดถึงในวิดีโอที่ผ่านมา แต่ผมจะบอกรายละเอียดในสไลด์ถัดไป

เริ่มจากวิธี Conversions from clicks โดยใช้ Google Click ID กันก่อน Google Ads ให้ ID ที่ไม่ซ้ำกับคุณ และ ID นี้เรียกว่า Google Click ID หรือเรียกสั้นๆ ว่า GCLID และมันไม่ซ้ำสำหรับทุกคลิกที่เข้ามาที่เว็บไซต์ของคุณจากโฆษณา ดังนั้น ถ้าคุณไปที่ Google ตอนนี้แล้วคลิกผลการค้นหาแบบสุ่ม คุณจะเห็นใน URL สุดท้ายในเบราว์เซอร์ของคุณว่า URL มีพารามิเตอร์ GCLID อยู่ และ ID นี้ผูกกับคลิกนั้นโดยเฉพาะ ข้อมูลทั้งหมดถูกบันทึกไว้ใน ID นี้ เช่น อุปกรณ์ที่คนใช้คลิกโฆษณาของคุณ ข้อมูลภูมิศาสตร์ แคมเปญ คำค้น (query) ที่ใช้จริง วันที่และเวลาของคลิก ทุกมิติผูกกับ ID นี้

เพื่อติดตาม offline conversions จากคลิกโดยใช้วิธีนี้ คุณจะต้องบันทึก Google Click ID นี้ พร้อมกับข้อมูล lead ที่คุณเก็บจากคนที่คลิกโฆษณาของคุณ เมื่อคนนั้นแปลง เช่น สมมติว่า lead เข้ามา สองสัปดาห์ผ่านไป คุณส่งใบเสนอราคา และคุณปิดดีลได้ คุณจะต้องใช้ ID นั้นเพื่ออัปโหลด offline conversion ของคุณไปยัง Google Ads และคุณต้องบอก Google เกี่ยวกับรายละเอียดบางอย่างของ offline conversion นั้น เช่น ประเภทของ conversion มันคือ conversion แบบไหน เกิดขึ้นเมื่อไหร่ เวลาที่เกิด conversion คือตอนไหน และมูลค่าเท่าไหร่ ในแง่ของรายได้ หรือ gross margin หรือคุณจะติดตามทั้งสองอย่างก็ได้ ซึ่งก็ง่ายมาก สิ่งเดียวที่คุณต้องทำคือบันทึก Google Click ID แยกมันออกมา แล้วส่งไปพร้อมกับข้อมูลของคุณ

จากนั้นเรามี Conversions from clicks โดยใช้ enhanced conversions for leads และนี่คือวิธีที่ง่ายขึ้นเพื่อติดตาม offline conversions แทนที่จะใช้ Google Click ID หรือ GCLID เป็นตัวระบุคลิกและคอนเวอร์ชันที่ไม่ซ้ำ คุณจะใช้ข้อมูล first-party ของลูกค้าเป็นตัวระบุที่ไม่ซ้ำ ถ้าคุณได้ทำตามวิดีโอก่อนๆ ที่ผมอธิบายวิธีตั้งค่า enhanced conversions คุณก็จะส่งข้อมูล first-party ไปกับการส่งฟอร์มของคุณอยู่แล้ว และมันใช้ข้อมูลนั้นที่ถูกบันทึกไว้ใน conversion pixel ของ Google Ads แล้ว เนื่องจากคุณส่งมันไปเพื่อจับคู่ offline conversions ของคุณ และการทำ offline conversions ด้วยวิธีนี้ไม่ต้องแก้ไขฟอร์ม lead ของคุณ เพราะคุณส่งข้อมูล first-party เป็นฟิลด์เพิ่มเติมไปกับแท็ก conversion tracking อยู่แล้ว CRM ก็ไม่ต้องรับ Google Click ID ด้วย ซึ่งทำให้มันง่ายกว่าวิธี Google Click ID มาก

มีข้อสังเกตสำคัญบางอย่างเกี่ยวกับ enhanced conversions for leads คือมันติดตั้งง่ายกว่ามาก แต่มันดูเหมือนจะมีประสิทธิภาพและความแม่นยำน้อยกว่าเมื่อเทียบกับวิธี Google Click ID ดังนั้น ถ้าเป็นไปได้ที่จะทำ offline conversions โดยใช้ Google Click ID นั่นคือ ถ้าคุณแก้ไขฟอร์มของคุณเพื่อส่ง Google Click ID เป็น hidden field ไปที่ CRM และอัปโหลด offline conversion โดยใช้ Google Click ID นั้นไปยัง Google Ads ผมก็จะใช้วิธีนี้มากกว่า enhanced conversions for leads แม้ว่า enhanced conversions for leads จะตั้งค่าได้ง่ายกว่ามาก ถ้าคุณตั้งค่า enhanced conversions ไว้แล้วก็ตาม

ในอีกไม่กี่วิดีโอถัดไป ผมจะทำวิดีโอแบบ over-the-shoulder เพื่อแสดงวิธีติดตั้งวิธี Google Click ID หรือวิธี enhanced conversions for leads โดยใช้เว็บไซต์ส่วนตัวของผมเป็นตัวอย่าง เจอกันในสองวิดีโอถัดไปครับ

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — คุณสามารถตั้งค่า offline conversion tracking (การติดตามคอนเวอร์ชันนอกเว็บไซต์)

**00:00:05** — ได้หลายวิธี และในคลิปนี้ผมจะบอกคุณถึงวิธีการติดตั้งทั้งหมดที่มีสำหรับ

**00:00:10** — OCT และจะบอกว่าเมื่อไหร่ควรใช้วิธีไหน เริ่มจากประเภทของ

**00:00:14** — offline conversion imports กันก่อน อย่างแรก เรามีฟังก์ชัน

**00:00:18** — native ที่สร้างไว้ใน Google Ads สำหรับการ import

**00:00:22** — conversion ถ้าคุณเลือกวิธีนี้ โดยพื้นฐานคุณจะมีวิธีการติดตั้งหลักสองแบบ

**00:00:27** — คุณสามารถเลือกแบบ Conversions from clicks โดยใช้

**00:00:30** — Google Click ID หรือที่รู้จักกันในชื่อ GCLID หรือคุณสามารถเลือกแบบ

**00:00:35** — enhanced conversions for leads วิธีการทั้งสองทำงานต่างกัน

**00:00:39** — และผมจะบอกความแตกต่างในสไลด์สองถัดไป จากนั้นเรามี

**00:00:43** — Google Ads Conversion Import แบบ built-in สำหรับ

**00:00:46** — Salesforce และ HubSpot ถ้าคุณใช้หนึ่งในสองเครื่องมือยอดนิยมเหล่านี้ที่ใช้กันแพร่หลาย

**00:00:52** — คุณสามารถซิงค์การ import conversion tracking ของคุณกับแพลตฟอร์ม

**00:00:57** — CRM เหล่านี้ได้โดยตรง และยังมีวิธี offline conversion

**00:01:01** — tracking ผ่าน Zapier ที่คุณสามารถเชื่อมต่อแอปทุกตัวเท่าที่มนุษย์รู้จักกับ

**00:01:06** — Google ได้ แต่คุณต้องสร้าง Zap ภายใน Zapier เพื่อให้มันทำงาน

**00:01:11** — ผมชอบใช้วิธี native ดังนั้นผมจะเลือกแบบ Conversions

**00:01:14** — from clicks โดยใช้ Google Click ID หรือแบบ enhanced

**00:01:18** — conversions for leads วิธี enhanced conversions

**00:01:21** — for leads นั้นติดตั้งง่ายที่สุด และนี่คือถ้าคุณได้ติดตั้ง

**00:01:25** — enhanced conversions ไว้แล้ว ซึ่งเราได้พูดถึงในวิดีโอที่ผ่านมา

**00:01:30** — แต่ผมจะบอกรายละเอียดในสไลด์ถัดไป เริ่มจากวิธี Conversions

**00:01:34** — from clicks โดยใช้ Google Click ID กันก่อน Google

**00:01:38** — Ads ให้ ID ที่ไม่ซ้ำกับคุณ และ ID นี้เรียกว่า Google

**00:01:41** — Click ID หรือเรียกสั้นๆ ว่า GCLID และมันไม่ซ้ำสำหรับทุกคลิกที่เข้ามาที่เว็บไซต์ของคุณจากโฆษณา

**00:01:48** — ดังนั้น ถ้าคุณไปที่ Google ตอนนี้แล้วคลิกผลการค้นหาแบบสุ่ม

**00:01:52** — คุณจะเห็นใน URL สุดท้ายในเบราว์เซอร์ของคุณว่า URL

**00:01:56** — มีพารามิเตอร์ GCLID อยู่ และ ID นี้ผูกกับคลิกนั้นโดยเฉพาะ

**00:02:00** — ข้อมูลทั้งหมดถูกบันทึกไว้ใน ID นี้ เช่น อุปกรณ์ที่คนใช้คลิกโฆษณาของคุณ

**00:02:05** — ข้อมูลภูมิศาสตร์ แคมเปญ คำค้น (query) ที่ใช้จริง

**00:02:09** — วันที่และเวลาของคลิก ทุกมิติผูกกับ ID นี้ เพื่อติดตาม

**00:02:12** — offline conversions จากคลิกโดยใช้วิธีนี้ คุณจะต้องบันทึก

**00:02:17** — Google Click ID นี้ พร้อมกับข้อมูล lead ที่คุณเก็บจากคนที่คลิกโฆษณาของคุณ

**00:02:22** — เมื่อคนนั้นแปลง เช่น สมมติว่า lead เข้ามา สองสัปดาห์ผ่านไป

**00:02:26** — คุณส่งใบเสนอราคา และคุณปิดดีลได้ คุณจะต้องใช้ ID

**00:02:30** — นั้นเพื่ออัปโหลด offline conversion ของคุณไปยัง

**00:02:33** — Google Ads และคุณต้องบอก Google เกี่ยวกับรายละเอียดบางอย่างของ

**00:02:37** — offline conversion นั้น เช่น ประเภทของ conversion

**00:02:41** — มันคือ conversion แบบไหน เกิดขึ้นเมื่อไหร่ เวลาที่เกิด

**00:02:45** — conversion คือตอนไหน และมูลค่าเท่าไหร่ ในแง่ของรายได้

**00:02:49** — หรือ gross margin หรือคุณจะติดตามทั้งสองอย่างก็ได้

**00:02:52** — ซึ่งก็ง่ายมาก สิ่งเดียวที่คุณต้องทำคือบันทึก Google

**00:02:56** — Click ID แยกมันออกมา แล้วส่งไปพร้อมกับข้อมูลของคุณ

**00:03:00** — จากนั้นเรามี Conversions from clicks โดยใช้ enhanced

**00:03:03** — conversions for leads และนี่คือวิธีที่ง่ายขึ้นเพื่อติดตาม

**00:03:08** — offline conversions แทนที่จะใช้ Google Click ID

**00:03:11** — หรือ GCLID เป็นตัวระบุคลิกและคอนเวอร์ชันที่ไม่ซ้ำ

**00:03:15** — คุณจะใช้ข้อมูล first-party ของลูกค้าเป็นตัวระบุที่ไม่ซ้ำ

**00:03:19** — ถ้าคุณได้ทำตามวิดีโอก่อนๆ ที่ผมอธิบายวิธีตั้งค่า

**00:03:22** — enhanced conversions คุณก็จะส่งข้อมูล first-party

**00:03:26** — ไปกับการส่งฟอร์มของคุณอยู่แล้ว และมันใช้ข้อมูลนั้นที่ถูกบันทึกไว้ใน

**00:03:31** — conversion pixel ของ Google Ads แล้ว เนื่องจากคุณส่งมันไปเพื่อจับคู่

**00:03:35** — offline conversions ของคุณ และการทำ offline conversions

**00:03:39** — ด้วยวิธีนี้ไม่ต้องแก้ไขฟอร์ม lead ของคุณ เพราะคุณส่งข้อมูล

**00:03:44** — first-party เป็นฟิลด์เพิ่มเติมไปกับแท็ก conversion

**00:03:47** — tracking อยู่แล้ว CRM ก็ไม่ต้องรับ Google Click

**00:03:51** — ID ด้วย ซึ่งทำให้มันง่ายกว่าวิธี Google Click ID

**00:03:54** — มาก มีข้อสังเกตสำคัญบางอย่างเกี่ยวกับ enhanced conversions

**00:03:58** — for leads คือมันติดตั้งง่ายกว่ามาก แต่มันดูเหมือนจะมีประสิทธิภาพและความแม่นยำน้อยกว่าเมื่อเทียบกับวิธี

**00:04:06** — Google Click ID ดังนั้น ถ้าเป็นไปได้ที่จะทำ offline

**00:04:10** — conversions โดยใช้ Google Click ID นั่นคือ ถ้าคุณแก้ไขฟอร์มของคุณเพื่อส่ง

**00:04:15** — Google Click ID เป็น hidden field ไปที่ CRM และอัปโหลด

**00:04:19** — offline conversion โดยใช้ Google Click ID นั้นไปยัง

**00:04:22** — Google Ads ผมก็จะใช้วิธีนี้มากกว่า enhanced conversions

**00:04:26** — for leads แม้ว่า enhanced conversions for leads

**00:04:30** — จะตั้งค่าได้ง่ายกว่ามาก ถ้าคุณตั้งค่า enhanced conversions

**00:04:34** — ไว้แล้วก็ตาม ในอีกไม่กี่วิดีโอถัดไป ผมจะทำวิดีโอแบบ

**00:04:38** — over-the-shoulder เพื่อแสดงวิธีติดตั้งวิธี Google

**00:04:41** — Click ID หรือวิธี enhanced conversions for leads

**00:04:45** — โดยใช้เว็บไซต์ส่วนตัวของผมเป็นตัวอย่าง เจอกันในสองวิดีโอถัดไปครับ

