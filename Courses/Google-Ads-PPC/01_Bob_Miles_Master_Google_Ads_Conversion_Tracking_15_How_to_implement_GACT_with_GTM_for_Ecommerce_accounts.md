---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 15 How to implement GACT with GTM for Ecommerce accounts"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 15 How to implement GACT with GTM for Ecommerce accounts

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_15_How_to_implement_GACT_with_GTM_for_Ecommerce_accounts.mp3]]

## 📝 คำแปล

# 01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_15_How_to_implement_GACT_with_GTM_for_Ecommerce_accounts

- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_15_How_to_implement_GACT_with_GTM_for_Ecommerce_accounts (วิดีโอท้องถิ่นในคอร์ส Google Ads PPC PayPerCall)
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~9-10 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ/STT)

---

## บทนำ

บทเรียนนี้ บ็อบ ไมลส์ (Bob Miles) สาธิตวิธีติดตั้ง Google Ads conversion tracking (การติดตามการแปลงของ Google Ads) แบบกำหนดเอง สำหรับร้านค้า อีคอมเมิร์ซ โดยใช้ Google Tag Manager (เครื่องมือจัดการแท็กของ Google) ร่วมกับตัวแปร data layer เช่น transaction ID และ transaction total พร้อมทั้งสาธิตการทดสอบ tag จริง ด้วย test order ผ่านโหมด Preview และหน้า /orders/confirmed

## คำแปลเต็ม

ในวิดีโอนี้ ผมอยากพูดถึง การติดตั้ง Google Ads conversion tracking แบบกำหนดเอง (custom implementation) สำหรับร้านค้า อีคอมเมิร์ซ ที่ออกแบบเฉพาะ
สำหรับร้านค้า อีคอมเมิร์ซ ส่วนใหญ่ คุณควรใช้ plug-in หรือ module เช่น WooCommerce จะดีกว่า
ไม่ว่าคุณจะใช้ platform อะไรก็ตาม
แต่บางครั้ง คุณไม่สามารถ หรือ ไม่ต้องการใช้ plugin คุณก็ต้องใช้ การติดตั้งแบบกำหนดเอง (custom implementation)
ก่อนอื่นเลย ถ้าคุณอยากทำแบบ custom คุณต้องมี data layer ที่ตั้งค่าไว้อย่างถูกต้อง
และสิ่งที่ผมมักจะทำ สำหรับการติดตั้งแบบ custom คือ การวางพื้นฐาน Google Ads conversion tracking บน data layer แบบ GA4
โดยอ้างอิงตามคู่มือการ implement (implementation guide)
ขอผมสาธิตตัวอย่าง วิธีที่เราตั้งค่าสิ่งนี้ สำหรับร้านของเราเอง เพราะเราใช้ e-comm tracking อยู่แล้ว
เราขายสินค้า อย่างเช่น Performance Max Mastery
และผู้คนสามารถเข้าถึงสินค้าเหล่านี้ ได้ง่ายๆ ด้วยการซื้อ ผ่านหน้า checkout ของเรา
สำหรับหน้า checkout นั้น เราใช้ผู้ให้บริการ บุคคลที่สาม (third-party provider) ที่ชื่อว่า Plug and Pay
เนื่องจากเป็นระบบของบุคคลที่สาม เราไม่สามารถแก้ไข data layer ได้ เราจึงขอให้พวกเขา เพิ่ม data layer บางตัว พร้อมข้อมูลบางอย่าง ที่เราจะนำไปใช้ กับ Google Ads conversion tracking tag
เพื่อให้เราส่งค่า value ได้
คือ มูลค่าของการขาย และ transaction ID ของการขาย
ขอผมพาคุณ ดูผ่านตัว debugger
นี่คือ test container
และขอพาคุณไปที่ หน้า checkout ของ Performance Max Mastery
นี่คือหน้าเพจ
ตรงนี้ ผมอยากให้คุณดู data layer และเราสามารถเจาะลึก ลงไปใน data layer เพื่อดูว่า ต้องใช้ตัวแปรใดบ้าง ใน Google Ads conversion tracking tag
เพื่อส่งข้อมูลสำคัญ เช่น value และ transaction ID
เอาเป็นว่า เรามาทำการทดสอบกัน
คำสั่งซื้อนี้ จะเป็น test order
กด Complete my purchase
Total
เอาล่ะ คำสั่งซื้อของผม กำลังได้รับการยืนยัน
Tag Assistant เชื่อมต่ออีกครั้งแล้ว
คุณอาจมองไม่เห็นบนหน้าจอ แต่ผมได้เข้าไปที่ URL /orders/confirmed
นี่คือ URL ที่เราสามารถใช้เป็น trigger สำหรับ Google Ads conversion tracking tag
กลับไปที่ debugger ใน Google Tag Manager กัน
อย่างที่คุณเห็น หน้า We Have Received Your Order ถูก trigger แล้ว โดยมี /orders/confirmed อยู่ใน URL
ต่อไป ขอดูที่ data layer
ภายใน data layer ตรงนี้ เราจะเห็นหลายสิ่ง
เราจะเห็น transaction ID
เราจะเห็นธุรกรรม ที่ไม่ซ้ำกัน
เราจะเห็นตัวแปร data layer ที่ชื่อว่า transaction และเห็น array ของ transaction products ที่แสดงราคา และ quantity
ดังนั้น สำหรับ Google Ads
conversion tracking ตอนนี้ เราต้องการแค่ transaction ID และ transaction total
เราจะจดค่าพวกนี้ไว้: transaction ID และ transaction total
อย่างที่คุณเห็น นี่คือค่าชุดแรก
ของตัวแปรทั้งหมด ใน data layer ก็ว่าได้
เพราะไม่มีโครงสร้างลำดับชั้น เหนือขึ้นไป
เราจึงสามารถใช้ตัวแปรเหล่านี้ได้ และ Google Tag Manager จะค้นหาค่าให้
ของตัวแปรสองตัวนี้
ต่อไป เรามากำหนดค่า tag กัน
เราต้องการตั้งค่าตัวแปร data layer เหล่านี้ เพราะภายใน Google Ads conversion tracking tag เราอยากใช้ค่า transaction total และ transaction ID
และเราต้องชี้ให้ Google Tag Manager ไปที่ตัวแปร data layer ที่ถูกต้อง เพื่อให้มันค้นหาค่าเจอ
เราจะสร้าง user-defined variable เพื่อทำสิ่งนี้
เราจะตั้งชื่อตัวแปรนี้ว่า DLV data layer variable
จากนั้น ผมจะเริ่มจาก transaction ID
นี่คือตัวแปรประเภท data layer variable
เราจะเลือก variable type แบบนั้น
ส่วนชื่อของตัวแปร [ฟังไม่ชัด]
และบันทึกเป็นตัวแปร
จากนั้นผมจะสร้างตัวแปรที่สอง
สำหรับ transaction total
ชื่อ DLV transaction ซึ่งเป็น data layer variable เช่นกัน
เสร็จแล้ว
แล้วก็ save
ตอนนี้เรามี transaction ID และ transaction
total ที่ตั้งค่าเรียบร้อยแล้ว
ทีนี้ เรามาดูที่แท็กของเรา
มาสร้าง Google Ads conversion tag ใหม่
ชื่อ Purchase
ตรงนี้ เราจะเลือก Google Ads conversion tracking tag
เราจะหา conversion ID และ conversion label
ผมได้สร้าง test conversion ไว้ ซึ่งเป็น purchase conversion
ไปที่หน้า tag setup ของ Google Tag Manager
ตรงนี้ คุณจะพบ conversion ID และ conversion label
ผมจะคัดลอกค่าพวกนี้ไป
เอาล่ะ ตอนนี้เรากำลังส่งข้อมูล และ conversion data ไปยัง conversion เฉพาะ ภายใน Google Ads
และตรงนี้ คุณจะเห็นช่องสามช่อง
ได้แก่ conversion value, transaction ID และ currency code
นี่คือตัวแปรที่สำคัญที่สุดสามตัว ที่คุณต้องตั้งค่า สำหรับ Google Ads conversion pixel ของร้านค้า e-comm
เริ่มจาก conversion value ก่อน
เราเพิ่งตั้งค่าตัวแปร data layer ไป และเราสามารถใช้ DLV transaction นี้ เพื่อส่ง conversion value
เราทำแบบเดียวกัน กับ transaction ID
เราสร้างตัวแปร data layer ไว้สำหรับอันนี้แล้ว
เสร็จแล้ว
จากนั้นก็เป็น currency code และร้านของเรา ใช้สกุลเงิน Euro เสมอ
เราสามารถใส่สกุลเงิน แบบ hard-coded ตรงนี้ได้เลย
แต่ถ้าลูกค้าสามารถใช้สกุลเงินอื่นได้ คุณต้องส่งค่านี้ ผ่าน data layer เป็นตัวแปรด้วย
แล้วก็ลิงก์ตัวแปร ในช่องนี้ด้วย
เอาล่ะ เสร็จแล้ว
เรากำลังส่ง transaction total, transaction ID และ currency code เป็น Euro
ทีนี้ เราจะใช้ trigger
ในเครื่องมือ debugging คุณเห็นแล้วว่า หน้า checkout success
เริ่มต้นด้วย /orders/confirmed
และผมได้สร้าง trigger ไว้แล้ว ซึ่งเป็น page view trigger ที่กรองจาก page path ที่เริ่มต้นด้วย /orders/ เราจึงใช้ตัวนี้ ที่สร้างไว้แล้วได้
คุณยังสามารถใช้ purchase event ได้ ถ้าคุณทำตามแนวทางมาตรฐาน
ถ้าคุณ implement GA4 e-commerce ตัวแปร data layer ทั้งหมดเหล่านี้ จะเป็นส่วนหนึ่ง
ของ GA4 purchase event ของคุณ
และเนื่องจากมันเป็นส่วนหนึ่งของ purchase event คุณจึงใช้ purchase เป็น trigger สำหรับ purchase tag ได้
มันไม่ได้ยากขนาดนั้น
เอาล่ะ
มาบันทึกกัน
เสร็จเรียบร้อย
มาส่ง (submit) กัน
publish แท็ก แล้วกลับไปที่หน้า debugging อีกครั้ง
เอาล่ะ
ผมจะปิดเซสชัน debugging ปัจจุบัน และเริ่มเซสชันใหม่ เพื่อตรวจสอบว่า การตั้งค่าที่เราเพิ่งทำ
เสร็จสิ้น ใช้งานได้หรือไม่
กด Preview
เข้าไปที่หน้า checkout เดิม
เอาล่ะ
ตรงนี้ควรแสดงว่าเราเชื่อมต่อแล้ว
เราเชื่อมต่อแล้ว
ภายใน debugger เช่นกัน
คุณจะเห็นว่า Google Ads Conversion Tag Purchase ยังไม่ถูก fire เพราะเรายังไม่ได้สั่งซื้อ
เรามาทำตอนนี้เลย
เอาล่ะ อันนี้ก็จะเป็น test order อีกครั้ง
กด Complete my purchase
เอาล่ะ คำสั่งซื้อของคุณ กำลังได้รับการยืนยัน
และเสร็จแล้ว
Debugger เชื่อมต่ออีกครั้ง
และเสร็จแล้ว
ตอนนี้เราอยู่ที่หน้า We Have Received Your Order และคุณจะเห็นว่าแท็ก BM ซึ่งคือ Google Ads Conversion Tag Purchase ถูก fire แล้ว
นั่นเป็นเพราะแท็กถูก trigger เมื่อหน้าเพจเริ่มต้นด้วย /orders/confirmed
เราสามารถคลิกที่ Google Ads Conversion Tag Purchase
และตรงนี้ คุณจะเห็นว่า มีพารามิเตอร์บางตัว ถูกส่งออกไป
คุณจะเห็นว่า เรากำลังส่ง conversion ที่ถูกต้อง และ currency เป็น Euro
คุณจะเห็นว่า เราชี้ไปที่ตัวแปร data layer ชื่อ transaction ID เพื่อส่ง transaction ID และชี้ไปที่ตัวแปร data layer ชื่อ transaction total เพื่อส่ง transaction total
ระบบทำงานได้อย่างที่ควรจะเป็น และนี่เป็นวิธีที่ง่ายมาก ในการส่งตัวแปรที่สำคัญที่สุด เช่น transaction ID ของคุณ
อย่าลืมส่ง ID ทุกครั้ง เพราะว่า
transaction ID นี้ จะถูก Google ใช้เพื่อ deduplicate ธุรกรรมบางรายการ
ถ้า conversion tag ของคุณถูก fire มากกว่าหนึ่งครั้ง Google Ads จะ deduplicate conversion นั้น และแสดงเฉพาะ conversion/order ที่เกิดขึ้นจริง เพียงรายการเดียว
ก็ประมาณนี้ครับ
ถ้าคุณมีคำถาม เกี่ยวกับการติดตั้ง custom e-comm ส่งข้อความมาหาผมได้
ย้ำอีกครั้ง ถ้าคุณใช้ platform ยอดนิยม
อย่างเช่น WooCommerce ขอแนะนำให้ใช้ plug-in สำหรับ tracking โดยเฉพาะ
ในอนาคตผมจะทำวิดีโอเกี่ยวกับ plug-in ที่ผมใช้บ่อยๆ ซึ่งจัดการโซลูชัน tracking ทั้งหมดของคุณ ภายใน 15 นาที ด้วยการตั้งค่า ซึ่งสะดวกกว่า การติดตั้งแบบ custom นี้มาก

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — ในวิดีโอนี้ ผมอยากพูดถึง การติดตั้ง Google Ads conversion

**00:00:04** — tracking แบบกำหนดเอง (custom implementation) สำหรับร้านค้า

**00:00:09** — อีคอมเมิร์ซ ที่ออกแบบเฉพาะ สำหรับร้านค้า อีคอมเมิร์ซ

**00:00:14** — ส่วนใหญ่ คุณควรใช้ plug-in หรือ module เช่น WooCommerce

**00:00:18** — จะดีกว่า ไม่ว่าคุณจะใช้ platform อะไรก็ตาม แต่บางครั้ง

**00:00:23** — คุณไม่สามารถ หรือ ไม่ต้องการใช้ plugin คุณก็ต้องใช้

**00:00:27** — การติดตั้งแบบกำหนดเอง (custom implementation) ก่อนอื่นเลย

**00:00:32** — ถ้าคุณอยากทำแบบ custom คุณต้องมี data layer ที่ตั้งค่าไว้อย่างถูกต้อง

**00:00:38** — และสิ่งที่ผมมักจะทำ สำหรับการติดตั้งแบบ custom คือ

**00:00:42** — การวางพื้นฐาน Google Ads conversion tracking บน

**00:00:46** — data layer แบบ GA4 โดยอ้างอิงตามคู่มือการ implement

**00:00:51** — (implementation guide) ขอผมสาธิตตัวอย่าง วิธีที่เราตั้งค่าสิ่งนี้

**00:00:56** — สำหรับร้านของเราเอง เพราะเราใช้ e-comm tracking

**00:01:00** — อยู่แล้ว เราขายสินค้า อย่างเช่น Performance Max

**00:01:04** — Mastery และผู้คนสามารถเข้าถึงสินค้าเหล่านี้ ได้ง่ายๆ

**00:01:09** — ด้วยการซื้อ ผ่านหน้า checkout ของเรา สำหรับหน้า

**00:01:13** — checkout นั้น เราใช้ผู้ให้บริการ บุคคลที่สาม (third-party

**00:01:18** — provider) ที่ชื่อว่า Plug and Pay เนื่องจากเป็นระบบของบุคคลที่สาม

**00:01:23** — เราไม่สามารถแก้ไข data layer ได้ เราจึงขอให้พวกเขา

**00:01:27** — เพิ่ม data layer บางตัว พร้อมข้อมูลบางอย่าง ที่เราจะนำไปใช้

**00:01:32** — กับ Google Ads conversion tracking tag เพื่อให้เราส่งค่า

**00:01:37** — value ได้ คือ มูลค่าของการขาย และ transaction ID

**00:01:41** — ของการขาย ขอผมพาคุณ ดูผ่านตัว debugger นี่คือ test

**00:01:45** — container และขอพาคุณไปที่ หน้า checkout ของ Performance

**00:01:50** — Max Mastery นี่คือหน้าเพจ ตรงนี้ ผมอยากให้คุณดู

**00:01:54** — data layer และเราสามารถเจาะลึก ลงไปใน data layer

**00:01:58** — เพื่อดูว่า ต้องใช้ตัวแปรใดบ้าง ใน Google Ads conversion

**00:02:03** — tracking tag เพื่อส่งข้อมูลสำคัญ เช่น value และ

**00:02:07** — transaction ID เอาเป็นว่า เรามาทำการทดสอบกัน คำสั่งซื้อนี้

**00:02:12** — จะเป็น test order กด Complete my purchase Total

**00:02:16** — เอาล่ะ คำสั่งซื้อของผม กำลังได้รับการยืนยัน Tag

**00:02:20** — Assistant เชื่อมต่ออีกครั้งแล้ว คุณอาจมองไม่เห็นบนหน้าจอ

**00:02:25** — แต่ผมได้เข้าไปที่ URL /orders/confirmed นี่คือ URL

**00:02:29** — ที่เราสามารถใช้เป็น trigger สำหรับ Google Ads conversion

**00:02:34** — tracking tag กลับไปที่ debugger ใน Google Tag Manager

**00:02:38** — กัน อย่างที่คุณเห็น หน้า We Have Received Your Order

**00:02:43** — ถูก trigger แล้ว โดยมี /orders/confirmed อยู่ใน

**00:02:47** — URL ต่อไป ขอดูที่ data layer ภายใน data layer ตรงนี้

**00:02:51** — เราจะเห็นหลายสิ่ง เราจะเห็น transaction ID เราจะเห็นธุรกรรม

**00:02:56** — ที่ไม่ซ้ำกัน เราจะเห็นตัวแปร data layer ที่ชื่อว่า

**00:03:00** — transaction และเห็น array ของ transaction products

**00:03:05** — ที่แสดงราคา และ quantity ดังนั้น สำหรับ Google Ads

**00:03:09** — conversion tracking ตอนนี้ เราต้องการแค่ transaction

**00:03:13** — ID และ transaction total เราจะจดค่าพวกนี้ไว้: transaction

**00:03:18** — ID และ transaction total อย่างที่คุณเห็น นี่คือค่าชุดแรก

**00:03:23** — ของตัวแปรทั้งหมด ใน data layer ก็ว่าได้ เพราะไม่มีโครงสร้างลำดับชั้น

**00:03:29** — เหนือขึ้นไป เราจึงสามารถใช้ตัวแปรเหล่านี้ได้ และ

**00:03:33** — Google Tag Manager จะค้นหาค่าให้ ของตัวแปรสองตัวนี้

**00:03:37** — ต่อไป เรามากำหนดค่า tag กัน เราต้องการตั้งค่าตัวแปร

**00:03:41** — data layer เหล่านี้ เพราะภายใน Google Ads conversion

**00:03:46** — tracking tag เราอยากใช้ค่า transaction total และ

**00:03:50** — transaction ID และเราต้องชี้ให้ Google Tag Manager

**00:03:54** — ไปที่ตัวแปร data layer ที่ถูกต้อง เพื่อให้มันค้นหาค่าเจอ

**00:03:59** — เราจะสร้าง user-defined variable เพื่อทำสิ่งนี้

**00:04:03** — เราจะตั้งชื่อตัวแปรนี้ว่า DLV data layer variable

**00:04:07** — จากนั้น ผมจะเริ่มจาก transaction ID นี่คือตัวแปรประเภท

**00:04:12** — data layer variable เราจะเลือก variable type แบบนั้น

**00:04:16** — ส่วนชื่อของตัวแปร [ฟังไม่ชัด] และบันทึกเป็นตัวแปร

**00:04:20** — จากนั้นผมจะสร้างตัวแปรที่สอง สำหรับ transaction

**00:04:24** — total ชื่อ DLV transaction ซึ่งเป็น data layer variable

**00:04:29** — เช่นกัน เสร็จแล้ว แล้วก็ save ตอนนี้เรามี transaction

**00:04:34** — ID และ transaction total ที่ตั้งค่าเรียบร้อยแล้ว

**00:04:38** — ทีนี้ เรามาดูที่แท็กของเรา มาสร้าง Google Ads conversion

**00:04:42** — tag ใหม่ ชื่อ Purchase ตรงนี้ เราจะเลือก Google

**00:04:46** — Ads conversion tracking tag เราจะหา conversion ID

**00:04:51** — และ conversion label ผมได้สร้าง test conversion

**00:04:55** — ไว้ ซึ่งเป็น purchase conversion ไปที่หน้า tag setup

**00:04:59** — ของ Google Tag Manager ตรงนี้ คุณจะพบ conversion

**00:05:03** — ID และ conversion label ผมจะคัดลอกค่าพวกนี้ไป เอาล่ะ

**00:05:08** — ตอนนี้เรากำลังส่งข้อมูล และ conversion data ไปยัง

**00:05:12** — conversion เฉพาะ ภายใน Google Ads และตรงนี้ คุณจะเห็นช่องสามช่อง

**00:05:17** — ได้แก่ conversion value, transaction ID และ currency

**00:05:22** — code นี่คือตัวแปรที่สำคัญที่สุดสามตัว ที่คุณต้องตั้งค่า

**00:05:26** — สำหรับ Google Ads conversion pixel ของร้านค้า e-comm

**00:05:31** — เริ่มจาก conversion value ก่อน เราเพิ่งตั้งค่าตัวแปร

**00:05:35** — data layer ไป และเราสามารถใช้ DLV transaction นี้

**00:05:39** — เพื่อส่ง conversion value เราทำแบบเดียวกัน กับ transaction

**00:05:44** — ID เราสร้างตัวแปร data layer ไว้สำหรับอันนี้แล้ว

**00:05:48** — เสร็จแล้ว จากนั้นก็เป็น currency code และร้านของเรา

**00:05:53** — ใช้สกุลเงิน Euro เสมอ เราสามารถใส่สกุลเงิน แบบ hard-coded

**00:05:58** — ตรงนี้ได้เลย แต่ถ้าลูกค้าสามารถใช้สกุลเงินอื่นได้

**00:06:02** — คุณต้องส่งค่านี้ ผ่าน data layer เป็นตัวแปรด้วย

**00:06:06** — แล้วก็ลิงก์ตัวแปร ในช่องนี้ด้วย เอาล่ะ เสร็จแล้ว

**00:06:10** — เรากำลังส่ง transaction total, transaction ID และ

**00:06:14** — currency code เป็น Euro ทีนี้ เราจะใช้ trigger ในเครื่องมือ

**00:06:19** — debugging คุณเห็นแล้วว่า หน้า checkout success เริ่มต้นด้วย

**00:06:24** — /orders/confirmed และผมได้สร้าง trigger ไว้แล้ว

**00:06:28** — ซึ่งเป็น page view trigger ที่กรองจาก page path

**00:06:32** — ที่เริ่มต้นด้วย /orders/ เราจึงใช้ตัวนี้ ที่สร้างไว้แล้วได้

**00:06:37** — คุณยังสามารถใช้ purchase event ได้ ถ้าคุณทำตามแนวทางมาตรฐาน

**00:06:42** — ถ้าคุณ implement GA4 e-commerce ตัวแปร data layer

**00:06:46** — ทั้งหมดเหล่านี้ จะเป็นส่วนหนึ่ง ของ GA4 purchase

**00:06:50** — event ของคุณ และเนื่องจากมันเป็นส่วนหนึ่งของ purchase

**00:06:55** — event คุณจึงใช้ purchase เป็น trigger สำหรับ purchase

**00:06:59** — tag ได้ มันไม่ได้ยากขนาดนั้น เอาล่ะ มาบันทึกกัน

**00:07:03** — เสร็จเรียบร้อย มาส่ง (submit) กัน publish แท็ก แล้วกลับไปที่หน้า

**00:07:09** — debugging อีกครั้ง เอาล่ะ ผมจะปิดเซสชัน debugging

**00:07:13** — ปัจจุบัน และเริ่มเซสชันใหม่ เพื่อตรวจสอบว่า การตั้งค่าที่เราเพิ่งทำ

**00:07:19** — เสร็จสิ้น ใช้งานได้หรือไม่ กด Preview เข้าไปที่หน้า

**00:07:23** — checkout เดิม เอาล่ะ ตรงนี้ควรแสดงว่าเราเชื่อมต่อแล้ว

**00:07:28** — เราเชื่อมต่อแล้ว ภายใน debugger เช่นกัน คุณจะเห็นว่า

**00:07:32** — Google Ads Conversion Tag Purchase ยังไม่ถูก fire

**00:07:36** — เพราะเรายังไม่ได้สั่งซื้อ เรามาทำตอนนี้เลย เอาล่ะ

**00:07:40** — อันนี้ก็จะเป็น test order อีกครั้ง กด Complete my

**00:07:45** — purchase เอาล่ะ คำสั่งซื้อของคุณ กำลังได้รับการยืนยัน

**00:07:49** — และเสร็จแล้ว Debugger เชื่อมต่ออีกครั้ง และเสร็จแล้ว

**00:07:54** — ตอนนี้เราอยู่ที่หน้า We Have Received Your Order

**00:07:58** — และคุณจะเห็นว่าแท็ก BM ซึ่งคือ Google Ads Conversion

**00:08:02** — Tag Purchase ถูก fire แล้ว นั่นเป็นเพราะแท็กถูก

**00:08:06** — trigger เมื่อหน้าเพจเริ่มต้นด้วย /orders/confirmed

**00:08:10** — เราสามารถคลิกที่ Google Ads Conversion Tag Purchase

**00:08:15** — และตรงนี้ คุณจะเห็นว่า มีพารามิเตอร์บางตัว ถูกส่งออกไป

**00:08:19** — คุณจะเห็นว่า เรากำลังส่ง conversion ที่ถูกต้อง และ

**00:08:24** — currency เป็น Euro คุณจะเห็นว่า เราชี้ไปที่ตัวแปร

**00:08:28** — data layer ชื่อ transaction ID เพื่อส่ง transaction

**00:08:32** — ID และชี้ไปที่ตัวแปร data layer ชื่อ transaction

**00:08:36** — total เพื่อส่ง transaction total ระบบทำงานได้อย่างที่ควรจะเป็น

**00:08:41** — และนี่เป็นวิธีที่ง่ายมาก ในการส่งตัวแปรที่สำคัญที่สุด

**00:08:46** — เช่น transaction ID ของคุณ อย่าลืมส่ง ID ทุกครั้ง

**00:08:50** — เพราะว่า transaction ID นี้ จะถูก Google ใช้เพื่อ

**00:08:54** — deduplicate ธุรกรรมบางรายการ ถ้า conversion tag

**00:08:58** — ของคุณถูก fire มากกว่าหนึ่งครั้ง Google Ads จะ deduplicate

**00:09:03** — conversion นั้น และแสดงเฉพาะ conversion/order ที่เกิดขึ้นจริง

**00:09:08** — เพียงรายการเดียว ก็ประมาณนี้ครับ ถ้าคุณมีคำถาม เกี่ยวกับการติดตั้ง

**00:09:14** — custom e-comm ส่งข้อความมาหาผมได้ ย้ำอีกครั้ง ถ้าคุณใช้

**00:09:19** — platform ยอดนิยม อย่างเช่น WooCommerce ขอแนะนำให้ใช้

**00:09:23** — plug-in สำหรับ tracking โดยเฉพาะ ในอนาคตผมจะทำวิดีโอเกี่ยวกับ

**00:09:28** — plug-in ที่ผมใช้บ่อยๆ ซึ่งจัดการโซลูชัน tracking

**00:09:32** — ทั้งหมดของคุณ ภายใน 15 นาที ด้วยการตั้งค่า ซึ่งสะดวกกว่า

**00:09:37** — การติดตั้งแบบ custom นี้มาก

