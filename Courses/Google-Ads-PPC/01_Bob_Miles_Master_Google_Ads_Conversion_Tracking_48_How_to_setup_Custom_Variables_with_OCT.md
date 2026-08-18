---
course: "Google Ads PPC"
lesson: "01 Bob Miles Master Google Ads Conversion Tracking 48 How to setup Custom Variables with OCT"
has_voiceover: true
has_subtitles: true
status: translated
synced_at: "2026-08-12"
tags: [thai-sub, course, google_ads_ppc]
---

# 01 Bob Miles Master Google Ads Conversion Tracking 48 How to setup Custom Variables with OCT

![[01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_48_How_to_setup_Custom_Variables_with_OCT.mp3]]

## 📝 คำแปล

# Bob Miles Master Google Ads Conversion Tracking 48 – วิธีตั้งค่า Custom Variables ร่วมกับ Offline Conversion Tracking (OCT)

- **วิดีโอต้นฉบับ:** local:01_Bob_Miles_Master_Google_Ads_Conversion_Tracking_48_How_to_setup_Custom_Variables_with_OCT (วิดีโอท้องถิ่นในคอร์ส Google Ads PPC PayPerCall)
- **ช่อง:** Google Ads PPC PayPerCall
- **ความยาว:** ~5 นาที
- **ภาษาต้นฉบับ:** อังกฤษ (คำบรรยายอัตโนมัติ)

---

## บทนำ
วิดีโอนี้เป็นบทเรียนที่ 48 จากคอร์ส Master Google Ads Conversion Tracking ของ Bob Miles ครับ
ผู้สอนอธิบายวิธีอัปโหลดข้อมูล custom variables (ตัวแปรที่กำหนดเอง) ผ่านการนำเข้าแบบ offline conversion tracking (OCT)
ไม่ว่าจะเป็นวิธี Google Click ID, Enhanced Conversions for Leads หรือ API integration
พร้อมข้อควรระวังสำคัญ เช่น ต้องสร้าง custom variables และ offline conversion action ให้พร้อมก่อนอัปโหลดเสมอครับ

## คำแปลเต็ม
ในวิดีโอนี้ผมจะพูดถึงวิธีอัปโหลดข้อมูล custom variables ผ่านการนำเข้าแบบ offline conversion tracking ครับ
ไม่สำคัญว่าคุณจะใช้วิธีไหนในการอัปโหลดข้อมูล offline conversion ของคุณ
ไม่ว่าจะเป็นการใช้ Google Click ID ที่คุณติดตาม บันทึก และส่งข้อมูล offline conversion ไปพร้อมกับพารามิเตอร์ Google Click ID
หรือจะทำผ่าน Enhanced Conversions for Leads ที่ใช้ first-party data (ข้อมูลของลูกค้าโดยตรง)
หรือจะใช้ API integration ก็ได้ทั้งหมดครับ

ตรงนี้ผมใช้เทมเพลตการนำเข้าแบบ offline conversion tracking import ที่อิงตามวิธี Enhanced Conversions for Leads ครับ
คุณจะเห็นอีเมลและเบอร์โทรศัพท์อยู่ในสองคอลัมน์แรก
ข้อมูลตรงนี้ถูก hash ไว้แล้ว เพราะเทมเพลตการนำเข้านี้จะถูกอัปโหลดอัตโนมัติผ่าน scheduled upload (การอัปโหลดตามกำหนดเวลา)
แต่ถ้าคุณทำ manual upload คุณไม่จำเป็นต้อง hash ข้อมูล first-party นี้ก็ได้ นี่เป็นแค่ตัวอย่างเท่านั้นครับ

ตรงนี้เรามีข้อมูล offline conversion tracking ทั่วไป
เราจะชี้ไปที่ offline conversion ที่เราต้องการส่ง custom variables ไป
ดังนั้นคุณต้องแน่ใจว่าชื่อ conversion (conversion name) นั้นเป็น offline conversion action จริงๆ ครับ
คุณไม่สามารถส่งข้อมูลเหล่านี้ไปยัง conversion action ทั่วไปของ Google Ads ได้ มันจะไม่ทำงานเด็ดขาด
คุณต้องสร้าง offline conversion ก่อน เพื่อที่จะอัปโหลดข้อมูล custom variable ไปยัง action นั้นได้
ใช้ชื่อ conversion ให้ถูกต้อง และชื่อต้องตรงกันแบบเป๊ะๆ ครับ

จากนั้นก็เป็นวันปิดดีล (date of closing) ดีลเกิดขึ้นเมื่อไหร่
มูลค่า (value) สกุลเงิน (currency) และอีกสามคอลัมน์สุดท้าย สิ่งเหล่านี้คือ custom variables ครับ
โดยปกติแล้ว offline conversion tracking อย่างน้อยสำหรับ enhanced conversions for leads ควรจำกัดอยู่แค่คอลัมน์ที่มีเบอร์โทรศัพท์
ซึ่งก็คือเทมเพลต enhanced conversions for leads ทั่วไปของคุณ
ส่วนคอลัมน์เหล่านี้เป็นคอลัมน์เพิ่มเติม และคุณสามารถใช้คอลัมน์เหล่านี้กับ Google Click ID import ใน Google Sheet หรือไฟล์ CSV ได้ด้วยครับ

สิ่งสำคัญคือคุณต้องใช้ชื่อ custom variable ให้ตรงกับชื่อที่ใช้ใน Google Ads ครับ
ขั้นแรกก่อนที่จะอัปโหลดเอกสารนี้จริงๆ คือคุณต้องสร้าง custom variable ก่อนการอัปโหลด
เราสามารถทำได้โดยไปที่ Tools แล้วก็ Conversions จากนั้นไปที่ Custom Variables ครับ
ตรงนี้ผมสร้าง custom variables ไว้แล้ว เพราะผมสอนวิธีสร้างให้ดูในวิดีโอก่อนหน้านี้แล้ว
แต่คุณต้องแน่ใจว่า custom variables เหล่านี้ถูกสร้างและเปิดใช้งาน (enabled) แล้ว
เพราะถ้ายังไม่ได้เปิดใช้งาน แล้วคุณพยายามอัปโหลด เทมเพลตการนำเข้าของคุณจะขึ้น error และ offline conversions จะไม่ถูกนำเข้าเลยครับ

วิธีนี้ต่างจากวิธี global site tag (gtag) เพราะถ้าคุณไม่สร้าง custom variables ก่อน
แล้วส่งข้อมูล custom variables ไปพร้อมกับ global site tag แบบ hard-coded
Google จะจดจำได้เองว่าคุณส่งข้อมูล custom variable ใหม่เข้ามา และคุณแค่ต้องไป activate มันเท่านั้น
แต่สำหรับวิธี offline conversions ใช้แบบนั้นไม่ได้ คุณต้องสร้าง custom variables ก่อน ซึ่งเราได้ทำไว้แล้วครับ

คุณจะเห็นว่าเราใช้ text strings (ข้อความ) ชุดเดียวกันในชีตของเรา
อย่าลืมเพิ่ม cv พร้อมเครื่องหมายจุดคู่ (double dot) นำหน้าชื่อ custom variable ด้วยครับ
ใส่ส่วนเล็กๆ นี้ก่อนชื่อ custom variable เช่น cv::hotel_name ครับ

จากนั้นก็ขึ้นอยู่กับคุณว่าจะส่งตัวแปรหรือค่าอะไรบ้าง
ตรงนี้ผมส่งชื่อโรงแรม เช่น NH Hilton
ผมส่ง room rate category (ประเภทอัตราค่าห้อง) ว่าเป็น standard room, economy room, comfort room หรือ premium
และส่ง loyalty status (สถานะสมาชิก) ของลูกค้าว่าเป็นลูกค้าประจำที่มาบ้างแต่ไม่บ่อยนัก
หรือเป็น ambassador ที่จองห้องทุกสัปดาห์ครับ

คุณควรวาง framework (กรอบโครงสร้าง) และกำหนดค่าที่เป็นไปได้ทั้งหมดที่จะใช้สำหรับ custom variables ของคุณครับ
เพราะข้อมูลทุกอย่างที่คุณอัปโหลดไปยัง Google Ads จะถูกจัดกลุ่มรวมกันในระดับหนึ่ง
ถ้าคุณมีโรงแรม 200 แห่ง คุณก็ไม่สามารถรวมชื่อโรงแรมเป็น custom variable ตัวเดียวได้
แต่สิ่งที่คุณทำได้คือสร้าง framework หรือการจัดหมวดหมู่สำหรับ room rate category หรือ loyalty status categories ของคุณ
ลองคิดแบบนี้เพื่อให้ทำงานกับ data points (จุดข้อมูล) ของคุณได้ง่ายขึ้นครับ

เมื่อทำเสร็จแล้ว และคุณกรอกค่าในทุกคอลัมน์สำหรับทุกตัวแปรแล้ว
คุณก็กลับไปที่ Google Ads อีกครั้ง ไปที่ Tools and Settings แล้วก็ Conversions
จากนั้นทางด้านซ้ายมือเลือก uploads
ตรงนี้คุณสามารถเลือกไฟล์ Google Sheet หรือไฟล์ CSV ที่ต้องการได้
แล้วคุณก็อัปโหลดด้วยตนเอง (manual upload) หรือจะสร้าง scheduled upload ก็ได้ครับ

เนื่องจากผม hash ข้อมูล first-party ไว้แล้ว ผมจะเลือก scheduled upload ครับ
ถ้าคุณเลือก Google Sheets คุณต้องเพิ่ม user ที่ระบบระบุลงในชีตด้วย
เลือกความถี่ เช่น ทุกคืน
แล้วเลือก Google Sheet ที่เชื่อมกับบัญชี Google ที่คุณล็อกอินอยู่ตอนนี้
จากนั้นก็ start และ preview การนำเข้าได้ครับ

ผมจะไม่ทำตอนนี้ เพราะนี่เป็นแค่ข้อมูลจำลอง (dummy data) และมันจะขึ้น error เยอะแยะ
แต่ถ้าคุณมีข้อมูล conversion จริงพร้อม first-party data ที่ใช้งานได้จริง
ถ้าคุณใช้วิธี enhanced conversions for leads หรือใช้ Google Click ID ถ้าคุณใช้วิธีนั้น
สิ่งนี้จะทำงานได้ลื่นไหลโดยไม่มีปัญหาอะไรเลยครับ

ก็ประมาณนี้ครับ ถ้าคุณเจอปัญหาอะไร บอกผมได้เลย ผมยินดีช่วยเสมอ
ผมคิดว่านี่เป็นวิธีที่ยอดเยี่ยมในการเพิ่ม data points ให้กับ offline conversions ของคุณ
เพื่อให้คุณใช้ข้อมูลเหล่านี้ในรายงาน Google Ads เพื่อหาคำตอบ และปรับปรุงแคมเปญของคุณให้ตรงกับธุรกิจจริง
ซึ่งสำคัญมากในปัจจุบันนี้ โชคดีนะครับ

---

*คำแปลนี้จัดทำขึ้นเพื่อการศึกษา/การใช้งานส่วนตัว อ้างอิงจากวิดีโอต้นฉบับ*

## ⏱️ ซับไตเติ้ล

**00:00:00** — ในวิดีโอนี้ผมจะพูดถึงวิธีอัปโหลดข้อมูล custom variables

**00:00:03** — ผ่านการนำเข้าแบบ offline conversion tracking ครับ

**00:00:06** — ไม่สำคัญว่าคุณจะใช้วิธีไหนในการอัปโหลดข้อมูล offline

**00:00:09** — conversion ของคุณ ไม่ว่าจะเป็นการใช้ Google Click

**00:00:12** — ID ที่คุณติดตาม บันทึก และส่งข้อมูล offline conversion

**00:00:15** — ไปพร้อมกับพารามิเตอร์ Google Click ID หรือจะทำผ่าน

**00:00:18** — Enhanced Conversions for Leads ที่ใช้ first-party

**00:00:21** — data (ข้อมูลของลูกค้าโดยตรง) หรือจะใช้ API integration

**00:00:24** — ก็ได้ทั้งหมดครับ ตรงนี้ผมใช้เทมเพลตการนำเข้าแบบ

**00:00:27** — offline conversion tracking import ที่อิงตามวิธี

**00:00:30** — Enhanced Conversions for Leads ครับ คุณจะเห็นอีเมลและเบอร์โทรศัพท์อยู่ในสองคอลัมน์แรก

**00:00:35** — ข้อมูลตรงนี้ถูก hash ไว้แล้ว เพราะเทมเพลตการนำเข้านี้จะถูกอัปโหลดอัตโนมัติผ่าน

**00:00:40** — scheduled upload (การอัปโหลดตามกำหนดเวลา) แต่ถ้าคุณทำ

**00:00:43** — manual upload คุณไม่จำเป็นต้อง hash ข้อมูล first-party

**00:00:46** — นี้ก็ได้ นี่เป็นแค่ตัวอย่างเท่านั้นครับ ตรงนี้เรามีข้อมูล

**00:00:50** — offline conversion tracking ทั่วไป เราจะชี้ไปที่

**00:00:52** — offline conversion ที่เราต้องการส่ง custom variables

**00:00:55** — ไป ดังนั้นคุณต้องแน่ใจว่าชื่อ conversion (conversion

**00:00:59** — name) นั้นเป็น offline conversion action จริงๆ ครับ

**00:01:02** — คุณไม่สามารถส่งข้อมูลเหล่านี้ไปยัง conversion action

**00:01:05** — ทั่วไปของ Google Ads ได้ มันจะไม่ทำงานเด็ดขาด คุณต้องสร้าง

**00:01:08** — offline conversion ก่อน เพื่อที่จะอัปโหลดข้อมูล

**00:01:11** — custom variable ไปยัง action นั้นได้ ใช้ชื่อ conversion

**00:01:14** — ให้ถูกต้อง และชื่อต้องตรงกันแบบเป๊ะๆ ครับ จากนั้นก็เป็นวันปิดดีล

**00:01:18** — (date of closing) ดีลเกิดขึ้นเมื่อไหร่ มูลค่า (value)

**00:01:21** — สกุลเงิน (currency) และอีกสามคอลัมน์สุดท้าย สิ่งเหล่านี้คือ

**00:01:25** — custom variables ครับ โดยปกติแล้ว offline conversion

**00:01:28** — tracking อย่างน้อยสำหรับ enhanced conversions for

**00:01:31** — leads ควรจำกัดอยู่แค่คอลัมน์ที่มีเบอร์โทรศัพท์ ซึ่งก็คือเทมเพลต

**00:01:35** — enhanced conversions for leads ทั่วไปของคุณ ส่วนคอลัมน์เหล่านี้เป็นคอลัมน์เพิ่มเติม

**00:01:40** — และคุณสามารถใช้คอลัมน์เหล่านี้กับ Google Click ID

**00:01:43** — import ใน Google Sheet หรือไฟล์ CSV ได้ด้วยครับ

**00:01:46** — สิ่งสำคัญคือคุณต้องใช้ชื่อ custom variable ให้ตรงกับชื่อที่ใช้ใน

**00:01:49** — Google Ads ครับ ขั้นแรกก่อนที่จะอัปโหลดเอกสารนี้จริงๆ

**00:01:53** — คือคุณต้องสร้าง custom variable ก่อนการอัปโหลด เราสามารถทำได้โดยไปที่

**00:01:57** — Tools แล้วก็ Conversions จากนั้นไปที่ Custom Variables

**00:02:00** — ครับ ตรงนี้ผมสร้าง custom variables ไว้แล้ว เพราะผมสอนวิธีสร้างให้ดูในวิดีโอก่อนหน้านี้แล้ว

**00:02:05** — แต่คุณต้องแน่ใจว่า custom variables เหล่านี้ถูกสร้างและเปิดใช้งาน

**00:02:09** — (enabled) แล้ว เพราะถ้ายังไม่ได้เปิดใช้งาน แล้วคุณพยายามอัปโหลด

**00:02:13** — เทมเพลตการนำเข้าของคุณจะขึ้น error และ offline conversions

**00:02:16** — จะไม่ถูกนำเข้าเลยครับ วิธีนี้ต่างจากวิธี global

**00:02:19** — site tag (gtag) เพราะถ้าคุณไม่สร้าง custom variables

**00:02:22** — ก่อน แล้วส่งข้อมูล custom variables ไปพร้อมกับ global

**00:02:26** — site tag แบบ hard-coded Google จะจดจำได้เองว่าคุณส่งข้อมูล

**00:02:29** — custom variable ใหม่เข้ามา และคุณแค่ต้องไป activate

**00:02:32** — มันเท่านั้น แต่สำหรับวิธี offline conversions ใช้แบบนั้นไม่ได้

**00:02:36** — คุณต้องสร้าง custom variables ก่อน ซึ่งเราได้ทำไว้แล้วครับ

**00:02:39** — คุณจะเห็นว่าเราใช้ text strings (ข้อความ) ชุดเดียวกันในชีตของเรา

**00:02:43** — อย่าลืมเพิ่ม cv พร้อมเครื่องหมายจุดคู่ (double dot)

**00:02:46** — นำหน้าชื่อ custom variable ด้วยครับ ใส่ส่วนเล็กๆ

**00:02:49** — นี้ก่อนชื่อ custom variable เช่น cv::hotel_name

**00:02:52** — ครับ จากนั้นก็ขึ้นอยู่กับคุณว่าจะส่งตัวแปรหรือค่าอะไรบ้าง

**00:02:55** — ตรงนี้ผมส่งชื่อโรงแรม เช่น NH Hilton ผมส่ง room

**00:02:58** — rate category (ประเภทอัตราค่าห้อง) ว่าเป็น standard

**00:03:01** — room, economy room, comfort room หรือ premium และส่ง

**00:03:04** — loyalty status (สถานะสมาชิก) ของลูกค้าว่าเป็นลูกค้าประจำที่มาบ้างแต่ไม่บ่อยนัก

**00:03:09** — หรือเป็น ambassador ที่จองห้องทุกสัปดาห์ครับ คุณควรวาง

**00:03:12** — framework (กรอบโครงสร้าง) และกำหนดค่าที่เป็นไปได้ทั้งหมดที่จะใช้สำหรับ

**00:03:16** — custom variables ของคุณครับ เพราะข้อมูลทุกอย่างที่คุณอัปโหลดไปยัง

**00:03:20** — Google Ads จะถูกจัดกลุ่มรวมกันในระดับหนึ่ง ถ้าคุณมีโรงแรม

**00:03:24** — 200 แห่ง คุณก็ไม่สามารถรวมชื่อโรงแรมเป็น custom

**00:03:27** — variable ตัวเดียวได้ แต่สิ่งที่คุณทำได้คือสร้าง

**00:03:29** — framework หรือการจัดหมวดหมู่สำหรับ room rate category

**00:03:33** — หรือ loyalty status categories ของคุณ ลองคิดแบบนี้เพื่อให้ทำงานกับ

**00:03:37** — data points (จุดข้อมูล) ของคุณได้ง่ายขึ้นครับ เมื่อทำเสร็จแล้ว

**00:03:40** — และคุณกรอกค่าในทุกคอลัมน์สำหรับทุกตัวแปรแล้ว คุณก็กลับไปที่

**00:03:44** — Google Ads อีกครั้ง ไปที่ Tools and Settings แล้วก็

**00:03:47** — Conversions จากนั้นทางด้านซ้ายมือเลือก uploads ตรงนี้คุณสามารถเลือกไฟล์

**00:03:51** — Google Sheet หรือไฟล์ CSV ที่ต้องการได้ แล้วคุณก็อัปโหลดด้วยตนเอง

**00:03:55** — (manual upload) หรือจะสร้าง scheduled upload ก็ได้ครับ

**00:03:58** — เนื่องจากผม hash ข้อมูล first-party ไว้แล้ว ผมจะเลือก

**00:04:01** — scheduled upload ครับ ถ้าคุณเลือก Google Sheets

**00:04:04** — คุณต้องเพิ่ม user ที่ระบบระบุลงในชีตด้วย เลือกความถี่

**00:04:07** — เช่น ทุกคืน แล้วเลือก Google Sheet ที่เชื่อมกับบัญชี

**00:04:11** — Google ที่คุณล็อกอินอยู่ตอนนี้ จากนั้นก็ start และ

**00:04:14** — preview การนำเข้าได้ครับ ผมจะไม่ทำตอนนี้ เพราะนี่เป็นแค่ข้อมูลจำลอง

**00:04:18** — (dummy data) และมันจะขึ้น error เยอะแยะ แต่ถ้าคุณมีข้อมูล

**00:04:21** — conversion จริงพร้อม first-party data ที่ใช้งานได้จริง

**00:04:24** — ถ้าคุณใช้วิธี enhanced conversions for leads หรือใช้

**00:04:27** — Google Click ID ถ้าคุณใช้วิธีนั้น สิ่งนี้จะทำงานได้ลื่นไหลโดยไม่มีปัญหาอะไรเลยครับ

**00:04:32** — ก็ประมาณนี้ครับ ถ้าคุณเจอปัญหาอะไร บอกผมได้เลย ผมยินดีช่วยเสมอ

**00:04:36** — ผมคิดว่านี่เป็นวิธีที่ยอดเยี่ยมในการเพิ่ม data points

**00:04:39** — ให้กับ offline conversions ของคุณ เพื่อให้คุณใช้ข้อมูลเหล่านี้ในรายงาน

**00:04:43** — Google Ads เพื่อหาคำตอบ และปรับปรุงแคมเปญของคุณให้ตรงกับธุรกิจจริง

**00:04:47** — ซึ่งสำคัญมากในปัจจุบันนี้ โชคดีนะครับ

