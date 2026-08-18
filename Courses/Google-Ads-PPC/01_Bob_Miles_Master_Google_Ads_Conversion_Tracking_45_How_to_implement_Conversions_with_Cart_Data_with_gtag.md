---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 45 How to implement Conversions with Cart Data with gtag"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-11"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 45 How to implement Conversions with Cart Data with gtag

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_45_How_to_implement_Conversions_with_Cart_Data_with_gtag.mp3]]

## 📝 คำแปล

# How to Implement Conversions with Cart Data with gtag

- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_45_How_to_implement_Conversions_with_Cart_Data_with_gtag
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~6 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)

---

## บทนำ
วิดีโอนี้เป็นบทเรียนจากคอร์ส Master Google Ads Conversion Tracking
ของ Bob Miles ครับ
สอนวิธีเพิ่มข้อมูลตะกร้าสินค้า (cart data)
ลงใน purchase conversion snippet แบบ hard-coded ด้วย gtag ครับ
ผู้สอนเตรียม template อีเมลสำหรับส่งให้ developer
พร้อมอธิบายพารามิเตอร์ที่ต้องส่ง เช่น discount, merchant ID,
feed country และ items array
รวมถึงวิธีตรวจสอบข้อมูลใน Google Ads ครับ

## คำแปลเต็ม
ถ้าคุณไม่ได้ใช้วิธีอื่น
คุณอาจใช้การติดตั้งแบบ hard-coded ด้วย Google Tag หรือ gtag ครับ
ถ้าคุณทำแบบนั้น
คุณควรใช้ purchase conversion event snippet แบบ hard-coded
บนหน้า checkout success ของคุณครับ
เพื่อส่งข้อมูล Conversion ทั้งหมดไปยัง Google Ads
ในวิดีโอนี้ ผมอยากอธิบายวิธีเพิ่มประสิทธิภาพ
ให้กับ purchase event conversion snippet ของคุณครับ
คุณเพิ่มข้อมูล และส่ง cart data
ไปยัง conversion tracking pixel ของ Google Ads ได้ด้วยครับ
ผมเตรียม template อีเมลง่ายๆ ไว้ให้ครับ
โดย developer ของคุณจะมีรายละเอียดครบ
ที่เขาหรือเธอต้องใช้ในการแก้ไขให้คุณครับ
สิ่งแรกที่ต้องทำคือ ใส่ URL ที่ conversion snippet ทำงานอยู่ครับ
ถ้าคุณรันร้าน Shopify, Magento 2 หรือ WooCommerce
คุณควรหาหน้า checkout success ได้
และบนหน้า checkout success นั้น
purchase event snippet ควรทำงาน
โดยส่งข้อมูล Conversion ไปยัง Google Ads ครับ
คุณควรช่วย developer โดยใส่ URL
ที่เขาต้องหาสำหรับ snippet ที่ต้องแก้ไขครับ
อย่าลืมใส่ URL ตรงนี้ครับ
จากนั้น ให้ developer ดูพารามิเตอร์ conversions with cart data
ที่ต้องส่งไปครับ
อย่างที่เห็น ผมใส่ demo script ไว้ครับ
จะเห็นว่านี่คือ gtag purchase event จริงๆ
ถูกส่งไปยังบัญชี Google Ads
พร้อมกับ transaction และสกุลเงิน
ทั้งหมดนี้คือ dummy data ครับ
อย่าลืมบอก developer ให้ข้ามส่วนนี้ไปครับ
มันมีไว้เพื่อให้เขารู้ว่าต้องใส่พารามิเตอร์ cart data ตรงไหนครับ
และตรงนี้คือจุดที่สนุกเริ่มต้นครับ
ในวิดีโอก่อนหน้า ที่ผมพูดถึง GTM
ผมพูดถึง variables อย่างละเอียดครับ
ถ้าอยากรู้ว่ามันทำงานยังไง และควรดูตรงไหน
ไปดูวิดีโอนั้นได้เลยครับ
แต่สำหรับตรงนี้ คุณต้องส่ง discount ถ้ามีครับ
ส่ง merchant ID ถ้าคุณมี merchant ID ครับ
ตั้งเป็นค่าคงที่ (static) ได้ครับ
ถ้าคุณมีหลาย merchant จะตั้งแบบ dynamic ก็ได้ครับ
เช่นเดียวกับ feed country และ feed language ครับ
อย่าลืมส่ง feed country และภาษาของผู้ใช้ครับ
คำสั่งซื้อถูกส่งไปที่ไหน
และภาษาของ feed ที่ถูกเรียกใช้คืออะไรครับ
คุณตั้งตามภาษาของหน้าร้าน (storefront) ได้
เก้าในสิบครั้ง หรือใช้ตาม domain ก็ได้ครับ
หรืออาจหาวิธีอื่นที่ทำให้เป็น dynamic ได้ครับ
คุณต้องตั้งเป็น dynamic ก็ต่อเมื่อมีมากกว่าหนึ่งค่าเท่านั้นครับ
ถ้าคุณส่งคำสั่งซื้อไปที่เดียว
และมีแค่หนึ่ง feed
ทั้งสองค่านี้ตั้งเป็น static ได้ครับ
แต่ถ้ามีมากกว่าหนึ่ง อย่าลืมตั้งเป็น dynamic
ไม่งั้น cart data ของคุณจะไม่แม่นยำครับ
แล้วขอย้ำอีกครั้ง
ส่ง items ในรูปแบบ array ครับ
ถ้ามีมากกว่าหนึ่งรายการที่ไม่ซ้ำ
ส่งใน array ครับ อย่างที่เห็นตรงนี้
สิ่งที่สำคัญมากคือ
ใช้ ID เดียวกับที่คุณใช้ในบัญชี Google Merchant Center ครับ
อย่าลืมตรวจสอบสามรอบ ไม่งั้นมันจะไม่ทำงานครับ
และนั่นคือทั้งหมดครับ
สิ่งสุดท้ายที่ต้องทำคือ ตรวจสอบว่า data points ทั้งหมด
เข้ามาในบัญชี Google Ads แล้วหรือยังครับ
ตรวจสอบได้โดยไปที่ product group report
ในแคมเปญ Performance Max
หรือ standard shopping ปกติ
เลือกคอลัมน์ cart data ใหม่
อย่าง gross cost of goods sold
แล้วดูว่ามีข้อมูลเข้ามาหรือไม่ครับ
ก่อนที่คุณจะเห็น cost of goods และ gross ได้
อย่าลืมส่ง cost of goods sold attribute
ภายใน product ใน Google Merchant Center ครับ
เพราะถ้าไม่มี cost of goods sold attribute
cart data จะไม่สามารถดึง cost of goods sold
จาก ID เหล่านั้นใน Google Merchant Center ได้ครับ
attribute นี้ควรมีอยู่แล้วครับ
ผมจะแปะลิงก์ไปยังบทความสนับสนุนของ Google ไว้ให้ครับ
วิธีเพิ่ม attribute นี้ใน feed
และวิธีจัดรูปแบบข้อมูลนี้ครับ
จบแค่นี้ครับ บอกผมได้เลยถ้ามีคำถามหรือปัญหาครับ
ผมคิดว่าเรื่องนี้ตรงไปตรงมามากครับ
ความมหัศจรรย์เดียวที่เกิดขึ้นตรงนี้
ควรอยู่ที่ฝั่ง developer
ที่สร้างและส่งพารามิเตอร์ของ Conversions with Cart Data ครับ
จบแค่นี้ครับ ขอให้โชคดีกับเรื่องนี้ครับ
และถ้ามีอะไร อย่าลืมติดต่อผมได้เลยครับ

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — ถ้าคุณไม่ได้ใช้วิธีอื่น คุณอาจใช้การติดตั้งแบบ hard-coded

**00:00:05** — ด้วย Google Tag หรือ gtag ครับ ถ้าคุณทำแบบนั้น คุณควรใช้

**00:00:11** — purchase conversion event snippet แบบ hard-coded

**00:00:16** — บนหน้า checkout success ของคุณครับ เพื่อส่งข้อมูล

**00:00:20** — Conversion ทั้งหมดไปยัง Google Ads ในวิดีโอนี้ ผมอยากอธิบายวิธีเพิ่มประสิทธิภาพ

**00:00:28** — ให้กับ purchase event conversion snippet ของคุณครับ

**00:00:33** — คุณเพิ่มข้อมูล และส่ง cart data ไปยัง conversion

**00:00:38** — tracking pixel ของ Google Ads ได้ด้วยครับ ผมเตรียม

**00:00:43** — template อีเมลง่ายๆ ไว้ให้ครับ โดย developer ของคุณจะมีรายละเอียดครบ

**00:00:50** — ที่เขาหรือเธอต้องใช้ในการแก้ไขให้คุณครับ สิ่งแรกที่ต้องทำคือ

**00:00:56** — ใส่ URL ที่ conversion snippet ทำงานอยู่ครับ ถ้าคุณรันร้าน

**00:01:02** — Shopify, Magento 2 หรือ WooCommerce คุณควรหาหน้า

**00:01:06** — checkout success ได้ และบนหน้า checkout success

**00:01:11** — นั้น purchase event snippet ควรทำงาน โดยส่งข้อมูล

**00:01:16** — Conversion ไปยัง Google Ads ครับ คุณควรช่วย developer

**00:01:21** — โดยใส่ URL ที่เขาต้องหาสำหรับ snippet ที่ต้องแก้ไขครับ

**00:01:27** — อย่าลืมใส่ URL ตรงนี้ครับ จากนั้น ให้ developer

**00:01:31** — ดูพารามิเตอร์ conversions with cart data ที่ต้องส่งไปครับ

**00:01:37** — อย่างที่เห็น ผมใส่ demo script ไว้ครับ จะเห็นว่านี่คือ

**00:01:42** — gtag purchase event จริงๆ ถูกส่งไปยังบัญชี Google

**00:01:47** — Ads พร้อมกับ transaction และสกุลเงิน ทั้งหมดนี้คือ

**00:01:52** — dummy data ครับ อย่าลืมบอก developer ให้ข้ามส่วนนี้ไปครับ

**00:01:58** — มันมีไว้เพื่อให้เขารู้ว่าต้องใส่พารามิเตอร์ cart

**00:02:03** — data ตรงไหนครับ และตรงนี้คือจุดที่สนุกเริ่มต้นครับ

**00:02:08** — ในวิดีโอก่อนหน้า ที่ผมพูดถึง GTM ผมพูดถึง variables

**00:02:13** — อย่างละเอียดครับ ถ้าอยากรู้ว่ามันทำงานยังไง และควรดูตรงไหน

**00:02:19** — ไปดูวิดีโอนั้นได้เลยครับ แต่สำหรับตรงนี้ คุณต้องส่ง

**00:02:24** — discount ถ้ามีครับ ส่ง merchant ID ถ้าคุณมี merchant

**00:02:29** — ID ครับ ตั้งเป็นค่าคงที่ (static) ได้ครับ ถ้าคุณมีหลาย

**00:02:34** — merchant จะตั้งแบบ dynamic ก็ได้ครับ เช่นเดียวกับ

**00:02:39** — feed country และ feed language ครับ อย่าลืมส่ง feed

**00:02:44** — country และภาษาของผู้ใช้ครับ คำสั่งซื้อถูกส่งไปที่ไหน

**00:02:50** — และภาษาของ feed ที่ถูกเรียกใช้คืออะไรครับ คุณตั้งตามภาษาของหน้าร้าน

**00:02:56** — (storefront) ได้ เก้าในสิบครั้ง หรือใช้ตาม domain

**00:03:01** — ก็ได้ครับ หรืออาจหาวิธีอื่นที่ทำให้เป็น dynamic

**00:03:06** — ได้ครับ คุณต้องตั้งเป็น dynamic ก็ต่อเมื่อมีมากกว่าหนึ่งค่าเท่านั้นครับ

**00:03:13** — ถ้าคุณส่งคำสั่งซื้อไปที่เดียว และมีแค่หนึ่ง feed

**00:03:18** — ทั้งสองค่านี้ตั้งเป็น static ได้ครับ แต่ถ้ามีมากกว่าหนึ่ง

**00:03:23** — อย่าลืมตั้งเป็น dynamic ไม่งั้น cart data ของคุณจะไม่แม่นยำครับ

**00:03:30** — แล้วขอย้ำอีกครั้ง ส่ง items ในรูปแบบ array ครับ

**00:03:34** — ถ้ามีมากกว่าหนึ่งรายการที่ไม่ซ้ำ ส่งใน array ครับ

**00:03:39** — อย่างที่เห็นตรงนี้ สิ่งที่สำคัญมากคือ ใช้ ID เดียวกับที่คุณใช้ในบัญชี

**00:03:46** — Google Merchant Center ครับ อย่าลืมตรวจสอบสามรอบ

**00:03:51** — ไม่งั้นมันจะไม่ทำงานครับ และนั่นคือทั้งหมดครับ สิ่งสุดท้ายที่ต้องทำคือ

**00:03:58** — ตรวจสอบว่า data points ทั้งหมด เข้ามาในบัญชี Google

**00:04:03** — Ads แล้วหรือยังครับ ตรวจสอบได้โดยไปที่ product group

**00:04:08** — report ในแคมเปญ Performance Max หรือ standard shopping

**00:04:14** — ปกติ เลือกคอลัมน์ cart data ใหม่ อย่าง gross cost

**00:04:18** — of goods sold แล้วดูว่ามีข้อมูลเข้ามาหรือไม่ครับ

**00:04:23** — ก่อนที่คุณจะเห็น cost of goods และ gross ได้ อย่าลืมส่ง

**00:04:29** — cost of goods sold attribute ภายใน product ใน Google

**00:04:34** — Merchant Center ครับ เพราะถ้าไม่มี cost of goods

**00:04:39** — sold attribute cart data จะไม่สามารถดึง cost of

**00:04:43** — goods sold จาก ID เหล่านั้นใน Google Merchant Center

**00:04:48** — ได้ครับ attribute นี้ควรมีอยู่แล้วครับ ผมจะแปะลิงก์ไปยังบทความสนับสนุนของ

**00:04:56** — Google ไว้ให้ครับ วิธีเพิ่ม attribute นี้ใน feed

**00:05:01** — และวิธีจัดรูปแบบข้อมูลนี้ครับ จบแค่นี้ครับ บอกผมได้เลยถ้ามีคำถามหรือปัญหาครับ

**00:05:08** — ผมคิดว่าเรื่องนี้ตรงไปตรงมามากครับ ความมหัศจรรย์เดียวที่เกิดขึ้นตรงนี้

**00:05:15** — ควรอยู่ที่ฝั่ง developer ที่สร้างและส่งพารามิเตอร์ของ

**00:05:20** — Conversions with Cart Data ครับ จบแค่นี้ครับ ขอให้โชคดีกับเรื่องนี้ครับ

**00:05:28** — และถ้ามีอะไร อย่าลืมติดต่อผมได้เลยครับ

