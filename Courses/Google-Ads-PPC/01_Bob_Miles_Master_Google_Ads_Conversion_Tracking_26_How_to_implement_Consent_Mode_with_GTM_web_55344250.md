---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 26 How to implement Consent Mode with GTM web 55344250"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 26 How to implement Consent Mode with GTM web 55344250

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_26_How_to_implement_Consent_Mode_with_GTM_web_55344250.mp3]]

## 📝 คำแปล

# 01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_26_How_to_implement_Consent_Mode_with_GTM_web_55344250
- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_26_How_to_implement_Consent_Mode_with_GTM_web_55344250
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~10 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)
---
## บทนำ
ในวิดีโอนี้ Bob Miles สอนวิธีติดตั้งและตั้งค่า Google Consent Mode (โหมดขอความยินยอม) ผ่าน Google Tag Manager (GTM) โดยใช้แพลตฟอร์ม CMP ที่มี community template เช่น Cookiebot พร้อมอธิบายความต่างระหว่าง built-in consent และ additional consent สำหรับแท็กของ Google กับแท็ก third-party อย่าง LinkedIn และปิดท้ายด้วยการสาธิตเช็คใน GTM debugger ว่าแท็กทำงานตามความยินยอมของผู้ใช้จริง
## คำแปลเต็ม
ในวิดีโอนี้ ผมจะแสดงวิธีตั้งค่า
และคอนฟิก Google Consent Mode แบบง่ายๆ
สิ่งสำคัญมากคือ คุณต้องใช้แพลตฟอร์ม CMP
ที่มี community template ให้ใช้งาน
ถ้าอยากรู้ว่า CMP ที่คุณใช้รองรับ Consent Mode ไหม
ให้ไปที่หน้า Google support
ที่ชื่อว่า Consent Mode on Websites and Mobile
และ Mobile Apps
ผมจะแปะลิงก์ไว้ให้ด้านล่างนี้
แล้วเลื่อนลงไปด้านล่างสุด
คุณจะเห็นหัวข้อ
consent management platform integrations
จะมีรายชื่อของ cookie management platforms
ทั้งหมดที่มี Tag Manager community template
ให้ดูที่เครื่องหมายถูกเป็นหลัก
ผมใช้ Cookiebot
ซึ่งผมว่าครบถ้วนและปรับแต่งได้ดีมาก
แต่คุณอาจจะใช้ CMP ตัวอื่นก็ได้
หรือคุณใช้ตัวอื่นอยู่แล้วก็ได้
ขอแค่เช็คว่า CMP ที่คุณจะใช้
มี community template ใน Tag Manager หรือเปล่า
ไปที่ Google Tag Manager กัน
การติดตั้ง CMP ใน GTM
ทำได้โดยการ import community template
วิธีทำคือไปที่เมนู Tags
แล้วกด New เพื่อสร้างแท็กใหม่
ปกติคุณจะเห็นรายการ tag types แบบ built-in
แต่ของที่เราต้องการ
อยู่ใน Community Template Gallery
ถ้าเปิดเข้าไป ก็ค้นหาด้วยคำว่า CMP ได้เลย
จะเห็นว่าผมเพิ่ม Cookiebot ไว้แล้ว
เพราะผมใช้มันอยู่
ต้องใช้ template นี้เพื่อตั้งค่า
Consent Mode integration ของผม
อย่างที่เห็น ยังมี template อื่นๆ ให้เลือกอีก
มีของ Usercentrics อยู่ตรงนี้
และ CookieScripts หรือ CookieYes อยู่ตรงนั้น
ขอแค่ CMP ที่คุณใช้มี template ให้ใช้งาน
ชีวิตคุณจะง่ายขึ้นเยอะเลย
ผม import template ของ Cookiebot ไว้แล้ว
และคอนฟิกเสร็จเรียบร้อยด้วย
การคอนฟิกค่อนข้างละเอียด
ผมแนะนำให้ทำตามคู่มือติดตั้ง
ของ CMP ที่คุณใช้โดยเฉพาะ
ไม่ใช่ตามวิดีโอนี้
วิดีโอนี้แค่ให้ภาพรวมคร่าวๆ
แต่ควรใช้คู่มือของแต่ละแพลตฟอร์ม
เพราะแต่ละตัวทำงานต่างกันนิดหน่อย
เพื่อให้ Cookiebot ทำงาน
ผมต้องใส่ ID ของผมเข้าไป
ในบัญชี cookiebot.com
จะมีสคริปต์เล็กๆ อันหนึ่ง
ซึ่งก็คือ domain group ID ของผม
ต้องเอาค่านั้นมาใส่
ซึ่งก็คือ Cookiebot ID นั่นเอง
เป็นสิ่งที่ชัดเจนที่สุด
การตั้งค่าหลักคือเปิดใช้งาน Google Consent Mode
ระบบจะส่ง Google API calls
ตามความยินยอมที่ผู้ใช้ให้
ยังมี setting อื่นๆ ให้คอนฟิกได้อีก
ใน template นี้
แต่ผมจะไม่ลงรายละเอียดตรงนั้น
ส่วน Triggers สำคัญมาก
ต้อง trigger CMP ของคุณ
ด้วยเหตุการณ์ consent initialization
หรือ cookie consent update
โดย consent update event ส่วนใหญ่
จะถูก push มาจาก CMP tag ของคุณ
มันจะส่งอัปเดตให้ Google Tag Manager
เมื่อมีการให้ความยินยอม
หรือเมื่อ consent เปลี่ยนไป
ว่าเป็นแบบไหน
เป็น ad storage, analytics storage
หรือไม่ยินยอมเลย
คุณใช้ cookie consent update เป็น trigger
ให้แท็กบางตัว fire ได้
อย่างที่เห็น ผมลิงก์มันกับ GA4
และ LinkedIn tag ของผมด้วย
เพราะอยากให้แท็กเหล่านี้ fire หรือ re-fire
ตาม consent ที่รู้ล่าสุด
ภายใน cookie consent update event
มาดู LinkedIn tag กัน
เริ่มจากดูฟีเจอร์ consent ก่อน
ก่อนเริ่มคอนฟิก ให้ไปที่ Admin
แล้วเข้า Container Settings
ตรงนี้จะมี setting เล็กๆ
ชื่อว่า Enable consent overview
หมายความว่าคุณจะมีปุ่ม consent
ให้คลิกดูได้
คุณจะเห็นว่าแท็กไหน
ยังไม่ได้รับ consent
และเห็นว่าให้ consent แบบไหนไปแล้ว
ตรงนี้มีสองแบบ
คือ Built-in consent กับ additional consent
Google tags ทั้งหมดจะมี built-in consent
คุณไม่ต้องคอนฟิกอะไรเพิ่ม
นอกจาก trigger ของ Google tags ที่มีอยู่
บางครั้งคุณไม่ต้องแก้แท็กอะไรเลย
เช่น Google Ads conversion tracking tag
เพราะมันปรับตาม consent ของผู้ใช้เอง
เช่น GA4 tag ของผม
มี built-in consent สองแบบ
คือ ad_storage กับ analytics_storage
ถ้าเลื่อนลงมาที่ consent settings
จะเห็นสองแบบนี้จริงๆ
คุณไม่ต้องคอนฟิก additional consent types เพิ่ม
ไม่จำเป็น
แต่เรายังมี LinkedIn tag อีกตัว
ตัวนี้ไม่มี built-in consent
เพราะมันไม่ใช่ native Google tag
และ Google ไม่รู้ว่ามันควรทำงานยังไง
คุณจึงต้องกำหนด additional consent types เอง
ถ้าคลิกแล้วเลื่อนลงมาด้านล่างของแท็ก
จะเห็นตัวเลือก require additional consent for tag
ให้คุณกำหนดเองได้
เพราะมันเป็น marketing pixel
ใช้ทำ remarketing audiences ด้วย
คุณต้องเลือกเป็น ad storage
ถ้าแท็กใช้เพื่อการวิเคราะห์ล้วนๆ
หรือใช้เพื่อ functionality
personalization หรือ security
ก็เลือกให้ถูกประเภท
แต่สำหรับแท็กนี้ ผมเลือก ad storage
แปลว่า LinkedIn tag จะ fire
บนทุก page views
เมื่อมีการให้ ad storage consent
เมื่อผู้ใช้ยินยอมให้ consent type นี้
ถ้าผู้ใช้ไม่ยินยอม Google จะรู้
Google Tag Manager จะรอ
consent type นี้ก่อน
ถ้าไม่ได้รับ ad storage
คุณตั้ง trigger ไว้ทุกหน้าได้
แต่แท็กจะไม่ fire
เพราะผู้ใช้ไม่ได้ให้ additional consent
สำหรับแท็กนี้ ถ้าเข้าใจนะ
หลักการทำงานก็ประมาณนี้
ง่ายและตรงไปตรงมา
ถ้ามี conversion pixel ใน GTM container
ก็แค่ trigger ด้วย event
เช่น purchase หรือ form submission
หรือ page view
คนที่เข้าหน้า checkout/success
ไม่ต้องทำ trigger ให้ซับซ้อน
ขอแค่มี built-in consent types
หรือ additional consent types
ที่คอนฟิกถูกต้อง
เช็ค consent overview ของคุณด้วย
ว่าใช้ additional consent ถูกต้อง
สำหรับ third-party pixels หรือเปล่า
ส่วน Google native tags
ไม่ต้องทำอะไรเลย
แค่คอนฟิก consent mode กับ CMP ให้ถูกต้อง
และเช็คกับคู่มือทางการ
ของ CMP ที่คุณใช้
มาดูใน debugger กัน
ว่าผมตั้งค่าได้ถูกต้องหรือเปล่า
มาดูการ fire ของ LinkedIn tag
มันควร fire เฉพาะเมื่อผมยินยอม
ตาม cookie/privacy policy
ลงมือกันเลย
ไปที่ Preview
จากนั้นไปที่เว็บของเรา
มันควรจะแสดงอะไรออกมา
เอาล่ะ ได้แล้ว
เราเชื่อมต่อกับ Tag Assistant แล้ว
ถ้าผมกลับมาที่ GTM
ผมเชื่อมต่อแล้วเช่นกัน
ตอนนี้จะเห็นว่า GA4 tag fire ไปแล้ว
แต่ยังไม่เต็มที่
เพราะมันยังรอ consent อยู่
แต่มันได้รับ ping แล้ว
มีผู้ใช้ใหม่เข้ามาที่เว็บ
มันกำลังรอ consent ก่อนจะ fire
ส่วน LinkedIn tag ยังไม่ fire เลย
ทั้งที่ trigger ของผม
คือ all pages หรือ cookie consent update
ซึ่งเป็นเงื่อนไขแบบ OR
ไม่ใช่ AND
ถ้าดูแค่ all pages แท็กนี้ควร fire แล้ว
แต่มันไม่ fire เพราะผมยังไม่ได้
ให้ความยินยอม
งั้นลองให้ consent กัน
ซึ่งซ่อนอยู่ข้างล่างนี้
กด Allow all
ทีนี้เราควรเห็น cookie consent update
ใน GTM จะเห็นว่า Preferences ถูกให้ consent แล้ว
consent statistics ก็เช่นกัน
รวมถึง marketing ด้วย
จะเห็นว่า LinkedIn Insight Tag ของผม fire แล้ว
เพราะผมให้ consent กับเว็บของผมเอง
ให้ fire แท็กนี้
หลักการทำงานคือแบบนี้
มันรอ consent types ที่ถูกต้องก่อนจะ fire
ถ้าไม่ได้ก็ไม่เป็นไร
เรายังมี conversion modeling
สำหรับ Google products
ซึ่งมีเฉพาะ Google tags
ไม่รวม third-party
แต่อย่างน้อยคุณก็ปฏิบัติตามกฎหมาย privacy
ลองไปตรวจสอบด้วยตัวเองดูนะครับ
ถึงตาคุณแล้ว
ไปคอนฟิกดู
ถ้าไม่มั่นใจร้อยเปอร์เซ็นต์
ให้ทดสอบกับ test container ก่อน
แล้วเช็คคู่มือติดตั้งของ CMP ที่คุณใช้อีกครั้ง
ว่าเขามี community template
ใน Google Tag Manager จริงหรือเปล่า
---
*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — ในวิดีโอนี้ ผมจะแสดงวิธีตั้งค่า และคอนฟิก Google

**00:00:04** — Consent Mode แบบง่ายๆ สิ่งสำคัญมากคือ คุณต้องใช้แพลตฟอร์ม

**00:00:10** — CMP ที่มี community template ให้ใช้งาน ถ้าอยากรู้ว่า

**00:00:15** — CMP ที่คุณใช้รองรับ Consent Mode ไหม ให้ไปที่หน้า

**00:00:20** — Google support ที่ชื่อว่า Consent Mode on Websites

**00:00:24** — and Mobile และ Mobile Apps ผมจะแปะลิงก์ไว้ให้ด้านล่างนี้

**00:00:30** — แล้วเลื่อนลงไปด้านล่างสุด คุณจะเห็นหัวข้อ consent

**00:00:35** — management platform integrations จะมีรายชื่อของ

**00:00:39** — cookie management platforms ทั้งหมดที่มี Tag Manager

**00:00:44** — community template ให้ดูที่เครื่องหมายถูกเป็นหลัก

**00:00:49** — ผมใช้ Cookiebot ซึ่งผมว่าครบถ้วนและปรับแต่งได้ดีมาก

**00:00:54** — แต่คุณอาจจะใช้ CMP ตัวอื่นก็ได้ หรือคุณใช้ตัวอื่นอยู่แล้วก็ได้

**00:01:00** — ขอแค่เช็คว่า CMP ที่คุณจะใช้ มี community template

**00:01:05** — ใน Tag Manager หรือเปล่า ไปที่ Google Tag Manager

**00:01:10** — กัน การติดตั้ง CMP ใน GTM ทำได้โดยการ import community

**00:01:15** — template วิธีทำคือไปที่เมนู Tags แล้วกด New เพื่อสร้างแท็กใหม่

**00:01:21** — ปกติคุณจะเห็นรายการ tag types แบบ built-in แต่ของที่เราต้องการ

**00:01:27** — อยู่ใน Community Template Gallery ถ้าเปิดเข้าไป

**00:01:32** — ก็ค้นหาด้วยคำว่า CMP ได้เลย จะเห็นว่าผมเพิ่ม Cookiebot

**00:01:37** — ไว้แล้ว เพราะผมใช้มันอยู่ ต้องใช้ template นี้เพื่อตั้งค่า

**00:01:43** — Consent Mode integration ของผม อย่างที่เห็น ยังมี

**00:01:47** — template อื่นๆ ให้เลือกอีก มีของ Usercentrics อยู่ตรงนี้

**00:01:53** — และ CookieScripts หรือ CookieYes อยู่ตรงนั้น ขอแค่

**00:01:58** — CMP ที่คุณใช้มี template ให้ใช้งาน ชีวิตคุณจะง่ายขึ้นเยอะเลย

**00:02:04** — ผม import template ของ Cookiebot ไว้แล้ว และคอนฟิกเสร็จเรียบร้อยด้วย

**00:02:10** — การคอนฟิกค่อนข้างละเอียด ผมแนะนำให้ทำตามคู่มือติดตั้ง

**00:02:15** — ของ CMP ที่คุณใช้โดยเฉพาะ ไม่ใช่ตามวิดีโอนี้ วิดีโอนี้แค่ให้ภาพรวมคร่าวๆ

**00:02:22** — แต่ควรใช้คู่มือของแต่ละแพลตฟอร์ม เพราะแต่ละตัวทำงานต่างกันนิดหน่อย

**00:02:29** — เพื่อให้ Cookiebot ทำงาน ผมต้องใส่ ID ของผมเข้าไป

**00:02:34** — ในบัญชี cookiebot.com จะมีสคริปต์เล็กๆ อันหนึ่ง

**00:02:38** — ซึ่งก็คือ domain group ID ของผม ต้องเอาค่านั้นมาใส่

**00:02:43** — ซึ่งก็คือ Cookiebot ID นั่นเอง เป็นสิ่งที่ชัดเจนที่สุด

**00:02:48** — การตั้งค่าหลักคือเปิดใช้งาน Google Consent Mode

**00:02:53** — ระบบจะส่ง Google API calls ตามความยินยอมที่ผู้ใช้ให้

**00:02:58** — ยังมี setting อื่นๆ ให้คอนฟิกได้อีก ใน template

**00:03:03** — นี้ แต่ผมจะไม่ลงรายละเอียดตรงนั้น ส่วน Triggers

**00:03:07** — สำคัญมาก ต้อง trigger CMP ของคุณ ด้วยเหตุการณ์ consent

**00:03:13** — initialization หรือ cookie consent update โดย consent

**00:03:18** — update event ส่วนใหญ่ จะถูก push มาจาก CMP tag ของคุณ

**00:03:23** — มันจะส่งอัปเดตให้ Google Tag Manager เมื่อมีการให้ความยินยอม

**00:03:29** — หรือเมื่อ consent เปลี่ยนไป ว่าเป็นแบบไหน เป็น ad

**00:03:34** — storage, analytics storage หรือไม่ยินยอมเลย คุณใช้

**00:03:38** — cookie consent update เป็น trigger ให้แท็กบางตัว

**00:03:43** — fire ได้ อย่างที่เห็น ผมลิงก์มันกับ GA4 และ LinkedIn

**00:03:48** — tag ของผมด้วย เพราะอยากให้แท็กเหล่านี้ fire หรือ

**00:03:53** — re-fire ตาม consent ที่รู้ล่าสุด ภายใน cookie consent

**00:03:58** — update event มาดู LinkedIn tag กัน เริ่มจากดูฟีเจอร์

**00:04:03** — consent ก่อน ก่อนเริ่มคอนฟิก ให้ไปที่ Admin แล้วเข้า

**00:04:08** — Container Settings ตรงนี้จะมี setting เล็กๆ ชื่อว่า

**00:04:13** — Enable consent overview หมายความว่าคุณจะมีปุ่ม consent

**00:04:18** — ให้คลิกดูได้ คุณจะเห็นว่าแท็กไหน ยังไม่ได้รับ consent

**00:04:24** — และเห็นว่าให้ consent แบบไหนไปแล้ว ตรงนี้มีสองแบบ

**00:04:28** — คือ Built-in consent กับ additional consent Google

**00:04:33** — tags ทั้งหมดจะมี built-in consent คุณไม่ต้องคอนฟิกอะไรเพิ่ม

**00:04:39** — นอกจาก trigger ของ Google tags ที่มีอยู่ บางครั้งคุณไม่ต้องแก้แท็กอะไรเลย

**00:04:46** — เช่น Google Ads conversion tracking tag เพราะมันปรับตาม

**00:04:51** — consent ของผู้ใช้เอง เช่น GA4 tag ของผม มี built-in

**00:04:56** — consent สองแบบ คือ ad_storage กับ analytics_storage

**00:05:01** — ถ้าเลื่อนลงมาที่ consent settings จะเห็นสองแบบนี้จริงๆ

**00:05:07** — คุณไม่ต้องคอนฟิก additional consent types เพิ่ม

**00:05:11** — ไม่จำเป็น แต่เรายังมี LinkedIn tag อีกตัว ตัวนี้ไม่มี

**00:05:16** — built-in consent เพราะมันไม่ใช่ native Google tag

**00:05:21** — และ Google ไม่รู้ว่ามันควรทำงานยังไง คุณจึงต้องกำหนด

**00:05:26** — additional consent types เอง ถ้าคลิกแล้วเลื่อนลงมาด้านล่างของแท็ก

**00:05:33** — จะเห็นตัวเลือก require additional consent for tag

**00:05:37** — ให้คุณกำหนดเองได้ เพราะมันเป็น marketing pixel ใช้ทำ

**00:05:42** — remarketing audiences ด้วย คุณต้องเลือกเป็น ad storage

**00:05:48** — ถ้าแท็กใช้เพื่อการวิเคราะห์ล้วนๆ หรือใช้เพื่อ functionality

**00:05:53** — personalization หรือ security ก็เลือกให้ถูกประเภท

**00:05:58** — แต่สำหรับแท็กนี้ ผมเลือก ad storage แปลว่า LinkedIn

**00:06:03** — tag จะ fire บนทุก page views เมื่อมีการให้ ad storage

**00:06:08** — consent เมื่อผู้ใช้ยินยอมให้ consent type นี้ ถ้าผู้ใช้ไม่ยินยอม

**00:06:15** — Google จะรู้ Google Tag Manager จะรอ consent type

**00:06:19** — นี้ก่อน ถ้าไม่ได้รับ ad storage คุณตั้ง trigger

**00:06:24** — ไว้ทุกหน้าได้ แต่แท็กจะไม่ fire เพราะผู้ใช้ไม่ได้ให้

**00:06:29** — additional consent สำหรับแท็กนี้ ถ้าเข้าใจนะ หลักการทำงานก็ประมาณนี้

**00:06:36** — ง่ายและตรงไปตรงมา ถ้ามี conversion pixel ใน GTM

**00:06:40** — container ก็แค่ trigger ด้วย event เช่น purchase

**00:06:45** — หรือ form submission หรือ page view คนที่เข้าหน้า

**00:06:50** — checkout/success ไม่ต้องทำ trigger ให้ซับซ้อน ขอแค่มี

**00:06:55** — built-in consent types หรือ additional consent types

**00:07:00** — ที่คอนฟิกถูกต้อง เช็ค consent overview ของคุณด้วย

**00:07:05** — ว่าใช้ additional consent ถูกต้อง สำหรับ third-party

**00:07:10** — pixels หรือเปล่า ส่วน Google native tags ไม่ต้องทำอะไรเลย

**00:07:15** — แค่คอนฟิก consent mode กับ CMP ให้ถูกต้อง และเช็คกับคู่มือทางการ

**00:07:22** — ของ CMP ที่คุณใช้ มาดูใน debugger กัน ว่าผมตั้งค่าได้ถูกต้องหรือเปล่า

**00:07:28** — มาดูการ fire ของ LinkedIn tag มันควร fire เฉพาะเมื่อผมยินยอม

**00:07:34** — ตาม cookie/privacy policy ลงมือกันเลย ไปที่ Preview

**00:07:39** — จากนั้นไปที่เว็บของเรา มันควรจะแสดงอะไรออกมา เอาล่ะ

**00:07:44** — ได้แล้ว เราเชื่อมต่อกับ Tag Assistant แล้ว ถ้าผมกลับมาที่

**00:07:50** — GTM ผมเชื่อมต่อแล้วเช่นกัน ตอนนี้จะเห็นว่า GA4 tag

**00:07:54** — fire ไปแล้ว แต่ยังไม่เต็มที่ เพราะมันยังรอ consent

**00:07:59** — อยู่ แต่มันได้รับ ping แล้ว มีผู้ใช้ใหม่เข้ามาที่เว็บ

**00:08:05** — มันกำลังรอ consent ก่อนจะ fire ส่วน LinkedIn tag

**00:08:09** — ยังไม่ fire เลย ทั้งที่ trigger ของผม คือ all pages

**00:08:14** — หรือ cookie consent update ซึ่งเป็นเงื่อนไขแบบ OR

**00:08:19** — ไม่ใช่ AND ถ้าดูแค่ all pages แท็กนี้ควร fire แล้ว

**00:08:24** — แต่มันไม่ fire เพราะผมยังไม่ได้ ให้ความยินยอม งั้นลองให้

**00:08:29** — consent กัน ซึ่งซ่อนอยู่ข้างล่างนี้ กด Allow all

**00:08:34** — ทีนี้เราควรเห็น cookie consent update ใน GTM จะเห็นว่า

**00:08:39** — Preferences ถูกให้ consent แล้ว consent statistics

**00:08:44** — ก็เช่นกัน รวมถึง marketing ด้วย จะเห็นว่า LinkedIn

**00:08:49** — Insight Tag ของผม fire แล้ว เพราะผมให้ consent กับเว็บของผมเอง

**00:08:55** — ให้ fire แท็กนี้ หลักการทำงานคือแบบนี้ มันรอ consent

**00:09:00** — types ที่ถูกต้องก่อนจะ fire ถ้าไม่ได้ก็ไม่เป็นไร

**00:09:05** — เรายังมี conversion modeling สำหรับ Google products

**00:09:10** — ซึ่งมีเฉพาะ Google tags ไม่รวม third-party แต่อย่างน้อยคุณก็ปฏิบัติตามกฎหมาย

**00:09:17** — privacy ลองไปตรวจสอบด้วยตัวเองดูนะครับ ถึงตาคุณแล้ว

**00:09:22** — ไปคอนฟิกดู ถ้าไม่มั่นใจร้อยเปอร์เซ็นต์ ให้ทดสอบกับ

**00:09:27** — test container ก่อน แล้วเช็คคู่มือติดตั้งของ CMP

**00:09:32** — ที่คุณใช้อีกครั้ง ว่าเขามี community template ใน

**00:09:36** — Google Tag Manager จริงหรือเปล่า

