---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 38 How to send over your transaction ID with GTM"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 38 How to send over your transaction ID with GTM

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_38_How_to_send_over_your_transaction_ID_with_GTM.mp3]]

## 📝 คำแปล

# How to Send Over Your Transaction ID with GTM

- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_38_How_to_send_over_your_transaction_ID_with_GTM
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~10 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)

---

## บทนำ
วิดีโอนี้จากคอร์ส Master Google Ads Conversion Tracking ของ Bob Miles สอนวิธีส่ง transaction ID ผ่าน Google Tag Manager ครับ
ผู้สอนสาธิตทั้งสองกรณี: อีคอมเมิร์ซ (ใช้ GA4 purchase event) และ lead gen (ใช้ฟอร์มสมัคร)
โดยอธิบายว่าการส่ง transaction ID แบบ dynamic จะช่วยให้ Google Ads ไม่นับ conversion ซ้ำซ้อน
จบด้วยการแนะนำ template อีเมลสำหรับแจ้ง developer ให้ติดตั้ง transaction ID ใน data layer ครับ

## คำแปลเต็ม
โอเค ในวิดีโอนี้
ผมอยากโชว์ให้คุณเห็นว่าคุณสามารถส่ง transaction ID
ผ่าน Google Tag Manager tag ของคุณได้ง่ายๆ แค่ไหน
และผมจะสาธิตสองตัวอย่าง
หนึ่งคือตัวอย่างอีคอมเมิร์ซ
และอีกหนึ่งคือตัวอย่าง lead gen
ทั้งสองแบบนี้
จะช่วยให้ผมโชว์ให้คุณเห็นวิธีทำได้ชัดเจนครับ
ก่อนอื่น ผมขอเริ่มด้วยตัวอย่างอีคอมเมิร์ซก่อน
ตรงนี้คุณเห็น landing page ของเราเอง
สำหรับ Google Ads Audit ที่ผู้คนสามารถซื้อได้
ทุกครั้งที่มีคนซื้อของ
transaction ID จะถูก trigger และถูกส่งออกไป
เราจึงต้องหา transaction ID เฉพาะนี้
ภายใน data layer code
แล้วใช้ data layer variable ตัวนี้
ส่งไปใน Google Ads GTM conversion tracking tags
เรามาดู GTM container ของเรากันก่อน
นี่คือตัวอย่าง container ของเว็บง่ายๆ
GTM container
ตรงนี้เราตั้งค่า GA4 purchase event ไว้แล้ว
ซึ่ง trigger บนหน้า checkout success
และเนื่องจากเราทำตามคำแนะนำของ GA4
เรากำลังส่ง transaction ID variable อยู่แล้ว
data layer บนหน้า checkout success
ส่งข้อมูลจำนวนมากอยู่แล้ว
ทั้งชื่อ transaction
และแน่นอน transaction ID
เราจึงมี data layer และ data layer variable อยู่แล้ว
ที่เราใช้สำหรับ GA4 purchase event
ผมขอโชว์เร็วๆ
เพื่อให้คุณเห็นว่าต้องหาที่ไหนใน data layer
และต้องมีอะไรอยู่ข้างใน
แล้วคุณจะรวม transaction ID
ใน Google Ads conversion tracking tag ได้ง่ายแค่ไหน
มาเริ่มกันเลย
เราจะใช้หน้า audit template ของเรา
ดูว่ามันเชื่อมต่อหรือยัง
มันเชื่อมต่อแล้วตรงนี้ และตรงนี้ด้วย
โอเค
ตอนนี้เราจะสั่งซื้อ template
อย่างที่เห็น debugger ยังเชื่อมต่ออยู่
มาใส่ข้อมูลจำลองกัน
ผมจะจ่ายด้วย iDEAL
นี่คือคำสั่งซื้อทดสอบ
เพราะผมล็อกอินอยู่
ผมจึงสั่งซื้อทดสอบได้ และซื้อให้เสร็จ
ผมจะตั้งค่าการทดสอบนี้ให้ fire สถานะ paid
แล้วกด continue
ตอนนี้เราอยู่บนหน้า orders confirmed แล้ว
debugger ยังเชื่อมต่ออยู่
และถ้าเรากลับไปที่ Google Tag Manager
เราควรเห็นว่า purchase event ของเรา
ถูก fire บนหน้านี้แล้ว
เราได้รับคำสั่งซื้อของคุณแล้ว
GA4 purchase event ถูก fire
และเนื่องจากเราอยู่บนหน้า success
data layer ควรเต็มไปด้วยข้อมูล transaction
ถ้าคุณเป็นอีคอมเมิร์ซ
คุณควรมีการติดตั้ง GA4 ที่ถูกต้องอยู่แล้ว
และถ้าคุณมีสิ่งนี้
คุณควรส่งข้อมูลอีคอมเมิร์ซผ่าน GA4 purchase
และข้อมูล transaction นี้
ควรจะอยู่ใน data layer
ถ้าคุณมีการติดตั้งผ่าน GTM
ตรงนี้เราเห็น transaction ID
นี่คือ data layer variable ที่เราต้องการ
และนี่คือ ID ที่ไม่ซ้ำกันต่อคำสั่งซื้อ
เราสามารถส่ง ID นี้ไปกับ Google Ads conversion tracking tag
เพื่อ deduplicate conversion
นี่คือ ID ที่เราตามหา
ถ้าเราไปที่ variables
แล้วเปิด GA4 event ของเรา
เราจะเห็นว่าเราใช้ transaction ID variable นี้อยู่แล้ว
Data layer variable ชื่อ transaction ID
เพื่อส่ง transaction ID ไปยัง GA4
เนื่องจากเรามีตัวนี้อยู่แล้ว
เราสามารถใช้ variable เดียวกันนี้
ส่งไปกับ Google Ads conversion tracking tag
ผมยังไม่มี tag นี้ติดตั้งไว้
เพราะเราไม่ได้ลงโฆษณาบน Google Ads
ขอโชว์ให้ดูว่าเป็นอย่างไร
เราสร้าง tag ใหม่ แล้วเลือก Google Ads Conversion Tracking
ถ้าคุณมี tag นี้อยู่แล้ว
คุณควรมี conversion linker ใน GTM
และคุณควรมี conversion ID ของคุณ
รวมถึง value ที่ต้องการส่งไปแล้ว
แต่สำหรับตอนนี้ ผมจะโชว์ให้เห็นว่า
คุณเลือก transaction ID ได้ตรงไหน
และส่งมันไปยังไง
ภายใน Google Ads conversion tracking
คุณจะเห็นสิ่งที่เรียกว่า transaction ID
และ Google ก็พูดเองว่า
การส่ง dynamic transaction ID ช่วยหลีกเลี่ยง
การนับ conversion ซ้ำซ้อน
ถ้ามี conversion สองครั้งสำหรับ conversion action เดียวกัน
ที่มี transaction ID เดียวกัน
Google Ads จะรู้ว่าครั้งที่สองเป็น duplicate
และจะไม่นับมัน
ตรงนี้เราจะเลือก data layer variable
ที่เรามีอยู่แล้ว
เพราะเราใช้มันสำหรับ GA4 purchase event
มันอยู่ตรงนี้
ก็แค่นี้แหละครับ
ถ้าคุณตั้งค่า Google Ads conversion ไว้แล้ว
คุณควรใช้สอง variable นี้อยู่แล้ว:
conversion ID ของคุณ และ transaction ID
แล้วคุณควรใส่ข้อมูลให้ Google Ads Conversion Tracking Tag
ให้มากที่สุดเท่าที่จะทำได้
ประมาณนี้ครับ
มันควรมีหน้าตาแบบนี้
มาดูตัวอย่าง lead gen กัน
ปิด debugger นี้ก่อน
แล้วไปที่เว็บไซต์ส่วนตัวของผม
เพราะนี่คือตัวอย่าง lead gen
ภายในฟอร์มเฉพาะนี้
เรากำลังส่ง Submission ID ที่ไม่ซ้ำกัน
และเพื่อให้มันทำงานได้
กับ Google Ads conversion tracking pixel ของ lead gen
คุณต้องสร้าง data layer variable
ที่ส่ง unique form submission ID
เพื่อให้คุณสามารถ
ใช้ variable นี้ใน Google Ads conversion tracking tag
ผมได้แก้ data layer ของผมแล้ว
ซึ่งจะถูก trigger เมื่อฟอร์มนี้ถูกส่ง
ใน event ที่ชื่อว่า form submission
หรือ form submitted
ภายในนั้น ผมส่งชื่อและอีเมล
เพื่อใช้ข้อมูลนี้สำหรับ enhanced conversion
แต่ผมยังส่งด้วยว่าเป็นลูกค้าใหม่หรือไม่
และผมยังส่ง unique form submission ID ด้วย
มาดีบักฟอร์มกันเร็วๆ
ดูว่าเราต้อง track variable ไหน
เราจะเข้า preview mode
เชื่อมต่อหน้า contact ของเรา
ไปเลย
มันเชื่อมต่อแล้ว
ตอนนี้ลองส่งฟอร์มดู
กดส่งคำขอติดต่อ
โอเค แค่นั้น
ตอนนี้ใน GTM
form submit event ถูก trigger แล้ว
ถ้าคุณต้องการส่ง form submission ID หรือ transaction ID
ต้องแน่ใจว่า unique ID นั้นพร้อมใช้งาน
ณ ช่วงเวลาที่เกิด conversion
ถ้าคุณส่ง unique ID หลังจาก trigger
ที่ใช้ fire tag ของคุณ
คุณจะพลาด
เพราะ Google Tag Manager หาค่าไม่เจอ
มันควรพร้อมใช้งานภายใน trigger เดียวกัน
หรือก่อนหน้านั้น
ผมใช้ form submit trigger นี้
เพื่อ fire Google Ads conversion tracking อย่างที่เห็น
และถ้าผมไปที่ data layer ของ data push นี้
คุณจะเห็นว่าผมส่งชื่อ
อีเมลของผู้กรอก
ผมส่ง contact form ID
แต่ ID นี้ไม่ unique
มัน unique สำหรับฟอร์มนี้
แต่มันเหมือนเดิมทุกการส่ง
สิ่งที่ผมทำคือผมส่ง submission ID
ที่ส่ง unique ID ตามจำนวนฟอร์มที่ถูกส่ง
การส่งแต่ละครั้งจะสร้าง unique ID
และผมสามารถใช้ ID นี้
ส่งไปกับ Google Ads conversion tracking tag
เราต้องหาโครงสร้าง (hierarchy)
ของ data layer ตัวนี้
โครงสร้างคือ form_submission
และข้างล่างเราเห็นค่า submission_id
เรารู้แล้วว่าจะสร้าง data layer variable ยังไง
เพื่อบอก GTM ว่าต้องหาค่าที่เราส่งไปตรงไหนใน data layer
มาคอนฟิกกัน
ก่อนอื่นไปที่ variables
เราต้องสร้าง variable ใหม่
เป็น user-defined variable
ชื่อ data layer form submission ID
ขอคัดลอกชื่อ variable ที่ถูกต้องกว่านี้มา
ได้แล้ว
การตั้งค่า variable เป็น data layer variable
เราจะใช้ submission ID
ผมพิมพ์ผิดตรงนั้น
อันนั้นไม่ถูกต้อง
เพราะเราต้องใช้ hierarchy
มันคือ meta.submission_id
เพราะมันเป็นส่วนหนึ่งของ meta
ถ้ามันอยู่ในแถวแรกของฟิลด์
เราอาจตั้งชื่อมันว่า submission
แต่ถ้าเราไม่ใส่ meta. ข้างหน้า
มันจะค้นหาแค่แถวแรก
และจะหาไม่เจอ
ตอนนี้ตั้งค่าถูกต้องแล้ว
meta.submission_id
ได้แล้ว
เราไปที่ tags
แล้วไปที่ Google Ads conversion tracking แบบ contact form
tag นี้ trigger
บน custom event form submit อย่างที่เห็นตรงนี้
และค่าควรพร้อมใช้งานใน data layer นั้น
อย่างที่เราเห็นใน data layer
ตอนนี้เราสามารถ
ส่ง transaction ID ไปกับ tag ของเราได้
คลิกที่ building block
แล้วเลือก DL form submission ID ที่เราสร้างใหม่
เนื่องจากเราเป็น lead gen
เราไม่ส่ง conversion value หรือ currency code
แต่ผมยังส่งข้อมูล new customer
และ first-party data อย่างชื่อ อีเมล และเบอร์โทร
เพื่อรวมไว้ใน enhanced conversion tracking
นี่คือการตั้งค่าที่สมบูรณ์
สำหรับ Google Ads conversion ของผม
ที่ตอนนี้ผมใช้ transaction ID
เพื่อ deduplicate form submissions
เรียบร้อยครับ
ถึงเวลา publish แล้วก็ publish
และทุกครั้งที่ Google Ads conversion tracking tag ยิง
transaction ID จะถูกส่งไปพร้อมกับ conversion ID และ conversion label
และ Google จะสามารถ deduplicate conversions ได้
แค่นั้นเอง
มันค่อนข้างง่ายที่จะใช้วิธีนี้
ถ้าคุณตั้งค่าผ่าน Google Tag Manager
สิ่งที่คุณต้องมีคือ transaction ID ใน data layer
แล้วใช้มันเป็น data layer variable
ภายใน Google Ads conversion tracking tag
ถ้าคุณยังไม่มี transaction ID
อย่าลืมใช้ email template briefing
ที่ผมสร้างไว้ให้คุณด้วย
คุณสามารถส่งมันให้ developer ของคุณ
เพื่อสั่งงานให้เขาติดตั้งสิ่งนี้
แค่นั้น
ในวิดีโอหน้า
เราจะมาดูวิธีตั้งค่านี้
ในการติดตั้งแบบ regular Google Ads conversion event snippet
ไปกันเลย
อืม

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — โอเค ในวิดีโอนี้ ผมอยากโชว์ให้คุณเห็นว่าคุณสามารถส่ง

**00:00:04** — transaction ID ผ่าน Google Tag Manager tag ของคุณได้ง่ายๆ

**00:00:08** — แค่ไหน และผมจะสาธิตสองตัวอย่าง หนึ่งคือตัวอย่างอีคอมเมิร์ซ

**00:00:13** — และอีกหนึ่งคือตัวอย่าง lead gen ทั้งสองแบบนี้ จะช่วยให้ผมโชว์ให้คุณเห็นวิธีทำได้ชัดเจนครับ

**00:00:20** — ก่อนอื่น ผมขอเริ่มด้วยตัวอย่างอีคอมเมิร์ซก่อน ตรงนี้คุณเห็น

**00:00:25** — landing page ของเราเอง สำหรับ Google Ads Audit ที่ผู้คนสามารถซื้อได้

**00:00:30** — ทุกครั้งที่มีคนซื้อของ transaction ID จะถูก trigger

**00:00:35** — และถูกส่งออกไป เราจึงต้องหา transaction ID เฉพาะนี้

**00:00:39** — ภายใน data layer code แล้วใช้ data layer variable

**00:00:43** — ตัวนี้ ส่งไปใน Google Ads GTM conversion tracking

**00:00:47** — tags เรามาดู GTM container ของเรากันก่อน นี่คือตัวอย่าง

**00:00:51** — container ของเว็บง่ายๆ GTM container ตรงนี้เราตั้งค่า

**00:00:55** — GA4 purchase event ไว้แล้ว ซึ่ง trigger บนหน้า checkout

**00:01:00** — success และเนื่องจากเราทำตามคำแนะนำของ GA4 เรากำลังส่ง

**00:01:04** — transaction ID variable อยู่แล้ว data layer บนหน้า

**00:01:08** — checkout success ส่งข้อมูลจำนวนมากอยู่แล้ว ทั้งชื่อ

**00:01:12** — transaction และแน่นอน transaction ID เราจึงมี data

**00:01:16** — layer และ data layer variable อยู่แล้ว ที่เราใช้สำหรับ

**00:01:21** — GA4 purchase event ผมขอโชว์เร็วๆ เพื่อให้คุณเห็นว่าต้องหาที่ไหนใน

**00:01:26** — data layer และต้องมีอะไรอยู่ข้างใน แล้วคุณจะรวม

**00:01:30** — transaction ID ใน Google Ads conversion tracking

**00:01:34** — tag ได้ง่ายแค่ไหน มาเริ่มกันเลย เราจะใช้หน้า audit

**00:01:38** — template ของเรา ดูว่ามันเชื่อมต่อหรือยัง มันเชื่อมต่อแล้วตรงนี้

**00:01:43** — และตรงนี้ด้วย โอเค ตอนนี้เราจะสั่งซื้อ template

**00:01:46** — อย่างที่เห็น debugger ยังเชื่อมต่ออยู่ มาใส่ข้อมูลจำลองกัน

**00:01:51** — ผมจะจ่ายด้วย iDEAL นี่คือคำสั่งซื้อทดสอบ เพราะผมล็อกอินอยู่

**00:01:56** — ผมจึงสั่งซื้อทดสอบได้ และซื้อให้เสร็จ ผมจะตั้งค่าการทดสอบนี้ให้

**00:02:01** — fire สถานะ paid แล้วกด continue ตอนนี้เราอยู่บนหน้า

**00:02:05** — orders confirmed แล้ว debugger ยังเชื่อมต่ออยู่

**00:02:09** — และถ้าเรากลับไปที่ Google Tag Manager เราควรเห็นว่า

**00:02:13** — purchase event ของเรา ถูก fire บนหน้านี้แล้ว เราได้รับคำสั่งซื้อของคุณแล้ว

**00:02:19** — GA4 purchase event ถูก fire และเนื่องจากเราอยู่บนหน้า

**00:02:23** — success data layer ควรเต็มไปด้วยข้อมูล transaction

**00:02:27** — ถ้าคุณเป็นอีคอมเมิร์ซ คุณควรมีการติดตั้ง GA4 ที่ถูกต้องอยู่แล้ว

**00:02:32** — และถ้าคุณมีสิ่งนี้ คุณควรส่งข้อมูลอีคอมเมิร์ซผ่าน

**00:02:36** — GA4 purchase และข้อมูล transaction นี้ ควรจะอยู่ใน

**00:02:40** — data layer ถ้าคุณมีการติดตั้งผ่าน GTM ตรงนี้เราเห็น

**00:02:44** — transaction ID นี่คือ data layer variable ที่เราต้องการ

**00:02:49** — และนี่คือ ID ที่ไม่ซ้ำกันต่อคำสั่งซื้อ เราสามารถส่ง

**00:02:53** — ID นี้ไปกับ Google Ads conversion tracking tag เพื่อ

**00:02:57** — deduplicate conversion นี่คือ ID ที่เราตามหา ถ้าเราไปที่

**00:03:02** — variables แล้วเปิด GA4 event ของเรา เราจะเห็นว่าเราใช้

**00:03:06** — transaction ID variable นี้อยู่แล้ว Data layer variable

**00:03:10** — ชื่อ transaction ID เพื่อส่ง transaction ID ไปยัง

**00:03:14** — GA4 เนื่องจากเรามีตัวนี้อยู่แล้ว เราสามารถใช้ variable

**00:03:19** — เดียวกันนี้ ส่งไปกับ Google Ads conversion tracking

**00:03:23** — tag ผมยังไม่มี tag นี้ติดตั้งไว้ เพราะเราไม่ได้ลงโฆษณาบน

**00:03:27** — Google Ads ขอโชว์ให้ดูว่าเป็นอย่างไร เราสร้าง tag

**00:03:31** — ใหม่ แล้วเลือก Google Ads Conversion Tracking ถ้าคุณมี

**00:03:36** — tag นี้อยู่แล้ว คุณควรมี conversion linker ใน GTM

**00:03:40** — และคุณควรมี conversion ID ของคุณ รวมถึง value ที่ต้องการส่งไปแล้ว

**00:03:45** — แต่สำหรับตอนนี้ ผมจะโชว์ให้เห็นว่า คุณเลือก transaction

**00:03:49** — ID ได้ตรงไหน และส่งมันไปยังไง ภายใน Google Ads conversion

**00:03:54** — tracking คุณจะเห็นสิ่งที่เรียกว่า transaction ID

**00:03:58** — และ Google ก็พูดเองว่า การส่ง dynamic transaction

**00:04:02** — ID ช่วยหลีกเลี่ยง การนับ conversion ซ้ำซ้อน ถ้ามี

**00:04:06** — conversion สองครั้งสำหรับ conversion action เดียวกัน

**00:04:10** — ที่มี transaction ID เดียวกัน Google Ads จะรู้ว่าครั้งที่สองเป็น

**00:04:15** — duplicate และจะไม่นับมัน ตรงนี้เราจะเลือก data layer

**00:04:19** — variable ที่เรามีอยู่แล้ว เพราะเราใช้มันสำหรับ GA4

**00:04:23** — purchase event มันอยู่ตรงนี้ ก็แค่นี้แหละครับ ถ้าคุณตั้งค่า

**00:04:28** — Google Ads conversion ไว้แล้ว คุณควรใช้สอง variable

**00:04:32** — นี้อยู่แล้ว: conversion ID ของคุณ และ transaction

**00:04:36** — ID แล้วคุณควรใส่ข้อมูลให้ Google Ads Conversion

**00:04:40** — Tracking Tag ให้มากที่สุดเท่าที่จะทำได้ ประมาณนี้ครับ

**00:04:44** — มันควรมีหน้าตาแบบนี้ มาดูตัวอย่าง lead gen กัน ปิด

**00:04:48** — debugger นี้ก่อน แล้วไปที่เว็บไซต์ส่วนตัวของผม เพราะนี่คือตัวอย่าง

**00:04:54** — lead gen ภายในฟอร์มเฉพาะนี้ เรากำลังส่ง Submission

**00:04:58** — ID ที่ไม่ซ้ำกัน และเพื่อให้มันทำงานได้ กับ Google

**00:05:02** — Ads conversion tracking pixel ของ lead gen คุณต้องสร้าง

**00:05:06** — data layer variable ที่ส่ง unique form submission

**00:05:10** — ID เพื่อให้คุณสามารถ ใช้ variable นี้ใน Google Ads

**00:05:14** — conversion tracking tag ผมได้แก้ data layer ของผมแล้ว

**00:05:18** — ซึ่งจะถูก trigger เมื่อฟอร์มนี้ถูกส่ง ใน event ที่ชื่อว่า

**00:05:23** — form submission หรือ form submitted ภายในนั้น ผมส่งชื่อและอีเมล

**00:05:28** — เพื่อใช้ข้อมูลนี้สำหรับ enhanced conversion แต่ผมยังส่งด้วยว่าเป็นลูกค้าใหม่หรือไม่

**00:05:35** — และผมยังส่ง unique form submission ID ด้วย มาดีบักฟอร์มกันเร็วๆ

**00:05:40** — ดูว่าเราต้อง track variable ไหน เราจะเข้า preview

**00:05:44** — mode เชื่อมต่อหน้า contact ของเรา ไปเลย มันเชื่อมต่อแล้ว

**00:05:48** — ตอนนี้ลองส่งฟอร์มดู กดส่งคำขอติดต่อ โอเค แค่นั้น

**00:05:52** — ตอนนี้ใน GTM form submit event ถูก trigger แล้ว

**00:05:56** — ถ้าคุณต้องการส่ง form submission ID หรือ transaction

**00:06:00** — ID ต้องแน่ใจว่า unique ID นั้นพร้อมใช้งาน ณ ช่วงเวลาที่เกิด

**00:06:05** — conversion ถ้าคุณส่ง unique ID หลังจาก trigger ที่ใช้

**00:06:09** — fire tag ของคุณ คุณจะพลาด เพราะ Google Tag Manager

**00:06:13** — หาค่าไม่เจอ มันควรพร้อมใช้งานภายใน trigger เดียวกัน

**00:06:17** — หรือก่อนหน้านั้น ผมใช้ form submit trigger นี้ เพื่อ

**00:06:21** — fire Google Ads conversion tracking อย่างที่เห็น

**00:06:25** — และถ้าผมไปที่ data layer ของ data push นี้ คุณจะเห็นว่าผมส่งชื่อ

**00:06:30** — อีเมลของผู้กรอก ผมส่ง contact form ID แต่ ID นี้ไม่

**00:06:35** — unique มัน unique สำหรับฟอร์มนี้ แต่มันเหมือนเดิมทุกการส่ง

**00:06:39** — สิ่งที่ผมทำคือผมส่ง submission ID ที่ส่ง unique

**00:06:43** — ID ตามจำนวนฟอร์มที่ถูกส่ง การส่งแต่ละครั้งจะสร้าง

**00:06:47** — unique ID และผมสามารถใช้ ID นี้ ส่งไปกับ Google

**00:06:51** — Ads conversion tracking tag เราต้องหาโครงสร้าง (hierarchy)

**00:06:55** — ของ data layer ตัวนี้ โครงสร้างคือ form_submission

**00:06:59** — และข้างล่างเราเห็นค่า submission_id เรารู้แล้วว่าจะสร้าง

**00:07:04** — data layer variable ยังไง เพื่อบอก GTM ว่าต้องหาค่าที่เราส่งไปตรงไหนใน

**00:07:10** — data layer มาคอนฟิกกัน ก่อนอื่นไปที่ variables เราต้องสร้าง

**00:07:14** — variable ใหม่ เป็น user-defined variable ชื่อ data

**00:07:18** — layer form submission ID ขอคัดลอกชื่อ variable ที่ถูกต้องกว่านี้มา

**00:07:24** — ได้แล้ว การตั้งค่า variable เป็น data layer variable

**00:07:28** — เราจะใช้ submission ID ผมพิมพ์ผิดตรงนั้น อันนั้นไม่ถูกต้อง

**00:07:33** — เพราะเราต้องใช้ hierarchy มันคือ meta.submission_id

**00:07:37** — เพราะมันเป็นส่วนหนึ่งของ meta ถ้ามันอยู่ในแถวแรกของฟิลด์

**00:07:41** — เราอาจตั้งชื่อมันว่า submission แต่ถ้าเราไม่ใส่

**00:07:45** — meta. ข้างหน้า มันจะค้นหาแค่แถวแรก และจะหาไม่เจอ

**00:07:49** — ตอนนี้ตั้งค่าถูกต้องแล้ว meta.submission_id ได้แล้ว

**00:07:53** — เราไปที่ tags แล้วไปที่ Google Ads conversion tracking

**00:07:57** — แบบ contact form tag นี้ trigger บน custom event

**00:08:01** — form submit อย่างที่เห็นตรงนี้ และค่าควรพร้อมใช้งานใน

**00:08:05** — data layer นั้น อย่างที่เราเห็นใน data layer ตอนนี้เราสามารถ

**00:08:10** — ส่ง transaction ID ไปกับ tag ของเราได้ คลิกที่ building

**00:08:15** — block แล้วเลือก DL form submission ID ที่เราสร้างใหม่

**00:08:19** — เนื่องจากเราเป็น lead gen เราไม่ส่ง conversion value

**00:08:23** — หรือ currency code แต่ผมยังส่งข้อมูล new customer

**00:08:27** — และ first-party data อย่างชื่อ อีเมล และเบอร์โทร

**00:08:31** — เพื่อรวมไว้ใน enhanced conversion tracking นี่คือการตั้งค่าที่สมบูรณ์

**00:08:37** — สำหรับ Google Ads conversion ของผม ที่ตอนนี้ผมใช้

**00:08:41** — transaction ID เพื่อ deduplicate form submissions

**00:08:45** — เรียบร้อยครับ ถึงเวลา publish แล้วก็ publish และทุกครั้งที่

**00:08:49** — Google Ads conversion tracking tag ยิง transaction

**00:08:53** — ID จะถูกส่งไปพร้อมกับ conversion ID และ conversion

**00:08:57** — label และ Google จะสามารถ deduplicate conversions

**00:09:01** — ได้ แค่นั้นเอง มันค่อนข้างง่ายที่จะใช้วิธีนี้ ถ้าคุณตั้งค่าผ่าน

**00:09:06** — Google Tag Manager สิ่งที่คุณต้องมีคือ transaction

**00:09:10** — ID ใน data layer แล้วใช้มันเป็น data layer variable

**00:09:15** — ภายใน Google Ads conversion tracking tag ถ้าคุณยังไม่มี

**00:09:19** — transaction ID อย่าลืมใช้ email template briefing

**00:09:23** — ที่ผมสร้างไว้ให้คุณด้วย คุณสามารถส่งมันให้ developer

**00:09:27** — ของคุณ เพื่อสั่งงานให้เขาติดตั้งสิ่งนี้ แค่นั้น

**00:09:31** — ในวิดีโอหน้า เราจะมาดูวิธีตั้งค่านี้ ในการติดตั้งแบบ

**00:09:35** — regular Google Ads conversion event snippet ไปกันเลย

**00:09:39** — อืม

