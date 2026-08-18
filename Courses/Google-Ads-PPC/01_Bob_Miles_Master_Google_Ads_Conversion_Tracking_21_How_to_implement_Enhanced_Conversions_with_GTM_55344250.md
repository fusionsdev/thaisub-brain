---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 21 How to implement Enhanced Conversions with GTM 55344250"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 21 How to implement Enhanced Conversions with GTM 55344250

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_21_How_to_implement_Enhanced_Conversions_with_GTM_55344250.mp3]]

## 📝 คำแปล

# 01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_21_How_to_implement_Enhanced_Conversions_with_GTM_55344250
- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_21_How_to_implement_Enhanced_Conversions_with_GTM_55344250
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~10 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)
---
## บทนำ
ในวิดีโอนี้ Bob Miles สอนวิธีตั้งค่า Enhanced Conversions (การแปลงข้อมูลผู้ใช้เพื่อเพิ่มความแม่นยำ) ผ่าน Google Tag Manager (GTM) โดยเริ่มจากให้ developer เตรียม first-party data ใน data layer จากนั้นสร้าง data layer variables แล้วลิงก์เข้ากับ Google Ads conversion tracking tag และปิดท้ายด้วยการ debug จริงเพื่อยืนยันว่าอีเมลและเบอร์โทรของผู้ใช้ถูกส่งอย่างถูกต้อง
## คำแปลเต็ม
ในวิดีโอนี้ ผมจะแสดงวิธีตั้งค่า
Enhanced Conversions ผ่าน Google Tag Manager
หรือที่เรียกว่า GTM
ก่อนจะตั้งค่าได้
คุณต้องมี first-party data
ที่เข้าถึงได้ภายใน data layer
ตรงนี้แหละที่ต้องพึ่งนักพัฒนา
อาจเป็นนักพัฒนาของลูกค้า
หรือในทีมของคุณเองก็ได้
แต่คุณต้องอาศัยนักพัฒนา
เพื่อทำให้ first-party data
ที่ส่งในฟอร์ม หรือหน้า checkout success
เข้าถึงได้สำหรับคุณ
ในฐานะ Google Ads specialist
เพราะคุณต้องใช้ข้อมูล
และ variables เหล่านี้
เพื่อคอนฟิก Google Tag Manager
เดี๋ยวผมจะโชว์วิธีทำ
ในช่วงหลังของวิดีโอนี้
ผมสร้าง email template ไว้ให้แล้ว
ใช้เป็นแม่แบบ
ส่ง brief ไปหานักพัฒนาได้เลย
สิ่งที่ต้องทำคือบอกนักพัฒนา
ว่าเหตุการณ์ไหนบ้าง
เช่น purchase event
หรือ form submission
ว่าต้องมี data layer event แบบไหน
หรือถ้ามี event อยู่แล้ว
ต้องเพิ่มข้อมูล user-provided
อย่างอีเมลหรือเบอร์โทรเข้าไป
คุณต้องดูว่า
มี event อย่าง purchase
หรือ form submission อยู่แล้วหรือเปล่า
ถ้ามี ให้ไฮไลต์ไว้ตรงนี้
ส่วนที่เขียนสีเหลือง
ให้แก้เป็นของคุณ
ถ้ายังไม่มี event
ก็ต้องสั่งให้นักพัฒนาสร้าง
แล้วต้องมั่นใจว่านักพัฒนา
ส่ง user-provided data มา
คือ first-party data
ที่บันทึกไว้ใน data layer ของเว็บลูกค้า
ผมแนะนำให้ใช้อีเมลของลูกค้าเป็นหลัก
ซึ่งจำเป็นสำหรับ Enhanced Conversions
ถ้าเป็นไปได้ก็เพิ่มเบอร์โทร
หรือแม้แต่ที่อยู่ด้วย
ผมส่วนใหญ่ใช้แค่อีเมลกับเบอร์โทร
เพราะข้อมูลเท่านี้
ก็เพียงพอในเกือบทุกกรณี
เมื่อนักพัฒนาใส่ data layer variables แล้ว
ไปที่ Google Tag Manager
เพื่อดูว่ามองเห็น variables เหล่านั้นไหม
ผมทำไว้ที่เว็บ bobmeier.nl/en
เป็นตัวอย่างให้ดูว่าใน GTM เป็นยังไง
ไปที่ Google Tag Manager กัน
ก่อนอื่น ผมจะโชว์วิธี debug
ว่า user-provided details
อย่างอีเมล ชื่อ และเบอร์โทร
ถูกส่งมาให้คุณจริงหรือเปล่า
มาเปิด debugger view กันก่อน
ไปที่เว็บส่วนตัวของผม
แล้วเชื่อมต่อ debugger
เช็คว่าเชื่อมต่อแล้ว
จากนั้นกรอกข้อมูลในฟอร์ม
แล้วกดส่งฟอร์มจริง
เมื่อฟอร์มส่ง event ไป
เราสามารถเช็คได้
ใน debugger ของ GTM
ตอนที่ผมส่งฟอร์ม
จะมี event ชื่อ submit ถูก push เข้ามา
และนี่คือ trigger
ของแท็กที่ผมอยากให้ fire
คือ Google Ads conversion tracking tag
ของฟอร์มติดต่อ
ถ้าดูที่ data ของ event นี้
เราจะเห็นค่าต่างๆ
ตรงนี้คือชื่อ
และตรงนี้มีรายละเอียดฟอร์ม
เราเห็นค่าของอีเมลที่กรอกไป
และค่าเบอร์โทรที่กรอกไปด้วย
ข้อมูลทั้งหมดอยู่ใน array
อย่างเรียบร้อย
ซึ่งส่วนใหญ่คุณทำเองไม่ได้
ต้องอาศัยนักพัฒนา
ช่วยเขียนโค้ด
และทำให้คุณเข้าถึงข้อมูลได้
จากนั้นผมก็สร้าง data layer variables
ในบัญชี GTM
เพื่อชี้ให้ GTM ไปที่ค่า
data layer variable ที่ถูกต้อง
แล้วส่งต่อใน Google Ads conversion tracking tag
มาดูโครงสร้าง hierarchy ของ array นี้ก่อน
จะเห็นว่าค่าแรกคือ fields
จากนั้นเป็น email
แล้วตามด้วย value
นี่คือ hierarchy
ของ data layer variable ของผม
fields.email.value
เบอร์โทรก็เหมือนกัน
คือ fields แล้วตามด้วยชื่อ field
ซึ่งเป็นชื่อสุ่ม
เพราะผมไม่ได้ตั้งชื่อมัน
แล้วปิดท้ายด้วย value เหมือนเดิม
แต่ละระดับคั่นด้วยจุด
เดี๋ยวจะโชว์ให้ดูว่า
มันทำงานใน GTM ยังไง
ไปที่ Google Tag Manager กัน
ไปที่เมนู Variables
แล้วเข้าไปที่ User-Defined Variables
เพราะเป็นตัวที่เราสร้างเอง
สร้าง data layer variable สำหรับอีเมลก่อน
ในส่วน variable configuration
เลือกประเภท Data Layer Variable
แล้วใส่ path ของ array
ที่ GTM จะหาค่าอีเมลเจอ
ซึ่งก็คือ fields.email.value
บางครั้งไม่มี hierarchy ซับซ้อน
แค่ variables หลายตัวในระดับเดียว
เช่น phone, address
ถ้าไม่มี hierarchy หรือ array
ก็อ้างอิงตัวแปรใน data layer ได้ตรงๆ
แต่กรณีผมมี hierarchy
ก็ต้องใช้จุดคั่น
นี่คือ data layer variable ของอีเมล
ต่อไปสร้างของเบอร์โทร
วางไว้ตรงนี้
ก็คือ fields แล้ว field ID
แล้วปิดด้วย value
ต่อไปก็บันทึก
ตอนนี้ user-defined variables ถูกบันทึกแล้ว
จากนั้นไปที่
Google Ads conversion tracking tag
ที่ตั้งไว้แล้ว
ต้องเช็คว่า ถ้าคุณใช้ event จริง
และเพิ่ม enhanced data ใน event นั้นแล้ว
ให้ใช้ event นั้นเป็น trigger
หรือใช้ event ที่เกิดทีหลัง
จุดที่ data layer variables ถูกส่ง
เพราะต้องเข้าถึงได้
ก่อนดึงออกมาจาก data layer
ผมชอบรวมไว้ใน trigger เดียวกัน
ใช้ trigger เดียวกับ purchase event
หรือ form submission อย่างที่เห็น
ไปที่ Google Ads conversion tracking tag ของผม
กดแก้ไข
จะเห็นตัวเลือก
Include user-provided data from your website
จากนั้นเลือก User-Provided Data Variables
สร้างใหม่
ตั้งชื่อว่า User Provided Data
จากนั้นแก้ variable configuration
ผมชอบใช้ manual configuration
เพราะมั่นใจได้ร้อยเปอร์เซ็นต์
ว่าจะไม่พลาด
ตรงนี้ให้ใช้ data layer variable email
ใส่ช่อง email
และตัวที่สร้างใหม่สำหรับเบอร์โทร
ใส่ช่อง phone
ก็แค่นี้แหละ
ถ้าต้องการ ก็ส่งข้อมูลอื่นๆ เพิ่มได้
แต่ผมไม่ค่อยใช้
เพราะอีเมลสำคัญที่สุด
อีเมลบวกเบอร์โทร
ทำให้ Google มี first-party data พอ
ที่จะ match conversion กับข้อมูลของเขา
เท่านั้นแหละ
บันทึกมัน
เห็นไหมว่ามันลิงก์
อยู่ใน advanced feature นี้แล้ว
บันทึกแท็ก
แล้ว submit และ publish
ตอนนี้เผยแพร่แล้ว
มาดูการ debug จริง
ว่าเวิร์กไหม
ปิด session เก่าก่อน
แล้วเปิดขึ้นมาใหม่
Preview หน้า contact อีกครั้ง
แล้วเชื่อมต่อ
เช็คว่า Tag Assistant เชื่อมต่อแล้ว
เชื่อมต่อแล้ว
กรอกฟอร์มใหม่อีกครั้ง
แล้วส่ง
ตอนนี้ event ถูกส่งแล้ว
เพราะฟอร์มส่งสำเร็จ
เช็คใน GTM debugger
จะเห็น form submit event
ใน data layer จะเห็นว่า
ค่าอีเมลและเบอร์โทร
ถูกส่งมาอย่างถูกต้อง
ไปที่ Variables
จะเห็นตัวแปรที่เราสร้างไว้
เห็น DLV email และ DLV phone number
ที่เพิ่งสร้างใน GTM
ตัวแปรเหล่านี้ถูกเติมค่า
ที่ถูกต้องจาก data layer
variables ของผมทำงานถูกต้อง
ต่อไปเปิดฟอร์มติดต่อของเรา
จะเห็นว่า enhanced conversions values
ถูกส่งไปด้วย
เห็นอีเมลและเบอร์โทรของผมตรงนี้
แปลว่าเราตั้งค่าและ debug สำเร็จ
ทุกอย่างทำงานดี
ทำงานได้สมบูรณ์ตามที่ควร
---
*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — ในวิดีโอนี้ ผมจะแสดงวิธีตั้งค่า Enhanced Conversions

**00:00:05** — ผ่าน Google Tag Manager หรือที่เรียกว่า GTM ก่อนจะตั้งค่าได้

**00:00:12** — คุณต้องมี first-party data ที่เข้าถึงได้ภายใน data

**00:00:18** — layer ตรงนี้แหละที่ต้องพึ่งนักพัฒนา อาจเป็นนักพัฒนาของลูกค้า

**00:00:25** — หรือในทีมของคุณเองก็ได้ แต่คุณต้องอาศัยนักพัฒนา

**00:00:30** — เพื่อทำให้ first-party data ที่ส่งในฟอร์ม หรือหน้า

**00:00:36** — checkout success เข้าถึงได้สำหรับคุณ ในฐานะ Google

**00:00:41** — Ads specialist เพราะคุณต้องใช้ข้อมูล และ variables

**00:00:47** — เหล่านี้ เพื่อคอนฟิก Google Tag Manager เดี๋ยวผมจะโชว์วิธีทำ

**00:00:54** — ในช่วงหลังของวิดีโอนี้ ผมสร้าง email template ไว้ให้แล้ว

**00:01:00** — ใช้เป็นแม่แบบ ส่ง brief ไปหานักพัฒนาได้เลย สิ่งที่ต้องทำคือบอกนักพัฒนา

**00:01:08** — ว่าเหตุการณ์ไหนบ้าง เช่น purchase event หรือ form

**00:01:14** — submission ว่าต้องมี data layer event แบบไหน หรือถ้ามี

**00:01:20** — event อยู่แล้ว ต้องเพิ่มข้อมูล user-provided อย่างอีเมลหรือเบอร์โทรเข้าไป

**00:01:28** — คุณต้องดูว่า มี event อย่าง purchase หรือ form submission

**00:01:35** — อยู่แล้วหรือเปล่า ถ้ามี ให้ไฮไลต์ไว้ตรงนี้ ส่วนที่เขียนสีเหลือง

**00:01:42** — ให้แก้เป็นของคุณ ถ้ายังไม่มี event ก็ต้องสั่งให้นักพัฒนาสร้าง

**00:01:49** — แล้วต้องมั่นใจว่านักพัฒนา ส่ง user-provided data

**00:01:54** — มา คือ first-party data ที่บันทึกไว้ใน data layer

**00:02:00** — ของเว็บลูกค้า ผมแนะนำให้ใช้อีเมลของลูกค้าเป็นหลัก

**00:02:05** — ซึ่งจำเป็นสำหรับ Enhanced Conversions ถ้าเป็นไปได้ก็เพิ่มเบอร์โทร

**00:02:13** — หรือแม้แต่ที่อยู่ด้วย ผมส่วนใหญ่ใช้แค่อีเมลกับเบอร์โทร

**00:02:19** — เพราะข้อมูลเท่านี้ ก็เพียงพอในเกือบทุกกรณี เมื่อนักพัฒนาใส่

**00:02:25** — data layer variables แล้ว ไปที่ Google Tag Manager

**00:02:31** — เพื่อดูว่ามองเห็น variables เหล่านั้นไหม ผมทำไว้ที่เว็บ

**00:02:37** — bobmeier.nl/en เป็นตัวอย่างให้ดูว่าใน GTM เป็นยังไง

**00:02:43** — ไปที่ Google Tag Manager กัน ก่อนอื่น ผมจะโชว์วิธี

**00:02:49** — debug ว่า user-provided details อย่างอีเมล ชื่อ

**00:02:54** — และเบอร์โทร ถูกส่งมาให้คุณจริงหรือเปล่า มาเปิด debugger

**00:03:00** — view กันก่อน ไปที่เว็บส่วนตัวของผม แล้วเชื่อมต่อ

**00:03:06** — debugger เช็คว่าเชื่อมต่อแล้ว จากนั้นกรอกข้อมูลในฟอร์ม

**00:03:12** — แล้วกดส่งฟอร์มจริง เมื่อฟอร์มส่ง event ไป เราสามารถเช็คได้

**00:03:19** — ใน debugger ของ GTM ตอนที่ผมส่งฟอร์ม จะมี event

**00:03:24** — ชื่อ submit ถูก push เข้ามา และนี่คือ trigger ของแท็กที่ผมอยากให้

**00:03:31** — fire คือ Google Ads conversion tracking tag ของฟอร์มติดต่อ

**00:03:38** — ถ้าดูที่ data ของ event นี้ เราจะเห็นค่าต่างๆ ตรงนี้คือชื่อ

**00:03:45** — และตรงนี้มีรายละเอียดฟอร์ม เราเห็นค่าของอีเมลที่กรอกไป

**00:03:51** — และค่าเบอร์โทรที่กรอกไปด้วย ข้อมูลทั้งหมดอยู่ใน

**00:03:56** — array อย่างเรียบร้อย ซึ่งส่วนใหญ่คุณทำเองไม่ได้

**00:04:01** — ต้องอาศัยนักพัฒนา ช่วยเขียนโค้ด และทำให้คุณเข้าถึงข้อมูลได้

**00:04:08** — จากนั้นผมก็สร้าง data layer variables ในบัญชี GTM

**00:04:14** — เพื่อชี้ให้ GTM ไปที่ค่า data layer variable ที่ถูกต้อง

**00:04:20** — แล้วส่งต่อใน Google Ads conversion tracking tag

**00:04:25** — มาดูโครงสร้าง hierarchy ของ array นี้ก่อน จะเห็นว่าค่าแรกคือ

**00:04:32** — fields จากนั้นเป็น email แล้วตามด้วย value นี่คือ

**00:04:38** — hierarchy ของ data layer variable ของผม fields.email.value

**00:04:44** — เบอร์โทรก็เหมือนกัน คือ fields แล้วตามด้วยชื่อ field

**00:04:50** — ซึ่งเป็นชื่อสุ่ม เพราะผมไม่ได้ตั้งชื่อมัน แล้วปิดท้ายด้วย

**00:04:57** — value เหมือนเดิม แต่ละระดับคั่นด้วยจุด เดี๋ยวจะโชว์ให้ดูว่า

**00:05:03** — มันทำงานใน GTM ยังไง ไปที่ Google Tag Manager กัน

**00:05:09** — ไปที่เมนู Variables แล้วเข้าไปที่ User-Defined Variables

**00:05:15** — เพราะเป็นตัวที่เราสร้างเอง สร้าง data layer variable

**00:05:21** — สำหรับอีเมลก่อน ในส่วน variable configuration เลือกประเภท

**00:05:28** — Data Layer Variable แล้วใส่ path ของ array ที่ GTM

**00:05:33** — จะหาค่าอีเมลเจอ ซึ่งก็คือ fields.email.value บางครั้งไม่มี

**00:05:40** — hierarchy ซับซ้อน แค่ variables หลายตัวในระดับเดียว

**00:05:46** — เช่น phone, address ถ้าไม่มี hierarchy หรือ array

**00:05:51** — ก็อ้างอิงตัวแปรใน data layer ได้ตรงๆ แต่กรณีผมมี

**00:05:57** — hierarchy ก็ต้องใช้จุดคั่น นี่คือ data layer variable

**00:06:03** — ของอีเมล ต่อไปสร้างของเบอร์โทร วางไว้ตรงนี้ ก็คือ

**00:06:08** — fields แล้ว field ID แล้วปิดด้วย value ต่อไปก็บันทึก

**00:06:14** — ตอนนี้ user-defined variables ถูกบันทึกแล้ว จากนั้นไปที่

**00:06:20** — Google Ads conversion tracking tag ที่ตั้งไว้แล้ว

**00:06:26** — ต้องเช็คว่า ถ้าคุณใช้ event จริง และเพิ่ม enhanced

**00:06:32** — data ใน event นั้นแล้ว ให้ใช้ event นั้นเป็น trigger

**00:06:38** — หรือใช้ event ที่เกิดทีหลัง จุดที่ data layer variables

**00:06:44** — ถูกส่ง เพราะต้องเข้าถึงได้ ก่อนดึงออกมาจาก data

**00:06:49** — layer ผมชอบรวมไว้ใน trigger เดียวกัน ใช้ trigger

**00:06:55** — เดียวกับ purchase event หรือ form submission อย่างที่เห็น

**00:07:01** — ไปที่ Google Ads conversion tracking tag ของผม กดแก้ไข

**00:07:07** — จะเห็นตัวเลือก Include user-provided data from your

**00:07:13** — website จากนั้นเลือก User-Provided Data Variables

**00:07:19** — สร้างใหม่ ตั้งชื่อว่า User Provided Data จากนั้นแก้

**00:07:24** — variable configuration ผมชอบใช้ manual configuration

**00:07:30** — เพราะมั่นใจได้ร้อยเปอร์เซ็นต์ ว่าจะไม่พลาด ตรงนี้ให้ใช้

**00:07:36** — data layer variable email ใส่ช่อง email และตัวที่สร้างใหม่สำหรับเบอร์โทร

**00:07:45** — ใส่ช่อง phone ก็แค่นี้แหละ ถ้าต้องการ ก็ส่งข้อมูลอื่นๆ

**00:07:51** — เพิ่มได้ แต่ผมไม่ค่อยใช้ เพราะอีเมลสำคัญที่สุด อีเมลบวกเบอร์โทร

**00:07:58** — ทำให้ Google มี first-party data พอ ที่จะ match

**00:08:03** — conversion กับข้อมูลของเขา เท่านั้นแหละ บันทึกมัน

**00:08:09** — เห็นไหมว่ามันลิงก์ อยู่ใน advanced feature นี้แล้ว

**00:08:14** — บันทึกแท็ก แล้ว submit และ publish ตอนนี้เผยแพร่แล้ว

**00:08:20** — มาดูการ debug จริง ว่าเวิร์กไหม ปิด session เก่าก่อน

**00:08:26** — แล้วเปิดขึ้นมาใหม่ Preview หน้า contact อีกครั้ง

**00:08:32** — แล้วเชื่อมต่อ เช็คว่า Tag Assistant เชื่อมต่อแล้ว

**00:08:37** — เชื่อมต่อแล้ว กรอกฟอร์มใหม่อีกครั้ง แล้วส่ง ตอนนี้

**00:08:43** — event ถูกส่งแล้ว เพราะฟอร์มส่งสำเร็จ เช็คใน GTM

**00:08:48** — debugger จะเห็น form submit event ใน data layer

**00:08:54** — จะเห็นว่า ค่าอีเมลและเบอร์โทร ถูกส่งมาอย่างถูกต้อง

**00:08:59** — ไปที่ Variables จะเห็นตัวแปรที่เราสร้างไว้ เห็น

**00:09:05** — DLV email และ DLV phone number ที่เพิ่งสร้างใน GTM

**00:09:10** — ตัวแปรเหล่านี้ถูกเติมค่า ที่ถูกต้องจาก data layer

**00:09:16** — variables ของผมทำงานถูกต้อง ต่อไปเปิดฟอร์มติดต่อของเรา

**00:09:22** — จะเห็นว่า enhanced conversions values ถูกส่งไปด้วย

**00:09:28** — เห็นอีเมลและเบอร์โทรของผมตรงนี้ แปลว่าเราตั้งค่าและ

**00:09:33** — debug สำเร็จ ทุกอย่างทำงานดี ทำงานได้สมบูรณ์ตามที่ควร

