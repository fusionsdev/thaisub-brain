---
videoId: "8VyHKDSyCCo"
title: "Claude Code Local Google Ads: Automate Everything ($730K Earned)"
channel: "Jono Catliff"
url: "https://www.youtube.com/watch?v=8VyHKDSyCCo"
published: ""
has_voiceover: false
status: translated
synced_at: "2026-10-08"
tags: [thai-sub, youtube]
---

# Claude Code Local Google Ads: Automate Everything ($730K Earned)

> [!info] แหล่งที่มา
> Jono Catliff · https://www.youtube.com/watch?v=8VyHKDSyCCo

## 📝 สรุป

# สรุป: Claude Code Local Google Ads: Automate Everything ($730K Earned)

- **ช่อง:** Jono Catliff · **ความยาว:** ~83 นาที · **ลิงก์:** https://www.youtube.com/watch?v=8VyHKDSyCCo

## ประเด็นหลัก

- Google Ads เป็นแค่ยอดภูเขาน้ำแข็ง — ต้องมีครบ 5 อย่างจึงสำเร็จ: โฆษณาที่ดี, landing page ที่แปลงยอด, การโทรติดตามเร็ว, ทักษะขาย และ analytics; เมตริกที่ Google โชว์ (CTR, conversion) เป็นแค่ตัวแทน ไม่ใช่กำไรจริงในกระเป๋า
- มี 3 ตำแหน่งโฆษณา: local search ads (โลคอล, ต้นทุนต่อลีดถูกกว่าครึ่งหนึ่ง แต่มีเพียง ~70 ประเภทธุรกิจที่เข้าเงื่อนไข), regular search ads และโฆษณาบน Google Maps
- ปัจจัยชี้ขาดของ local search ads คือรีวิว: จำนวน คะแนน และความถี่ในการได้รีวิวใหม่ (review velocity) — สูตรจัดอันดับคือ งบ × ความตอบสนอง × รีวิว × รูปภาพ
- ระบบเก็บรีวิวอัตโนมัติ: ฟอร์ม Next.js สองคำถาม (1-5 ดาว + feedback) → ถ้า 4-5 ดาวพาไปทิ้งรีวิว Google, ถ้า 1-3 ดาวส่งเข้า Slack ผ่าน make.com เพื่อจัดการภายใน
- Keyword research: ต้องเลือก keyword ที่มี intent ซื้อจริง (emergency plumber, plumber near me) หลีกเลี่ยงคำหางาน/คู่แข่ง/DIY และใช้ phrase match เป็นหลัก
- กลยุทธ์ single keyword ad groups: สร้าง landing page เฉพาะบริการ × เมือง ให้คำค้น โฆษณา หน้าเว็บ อีเมล และสายขายสอดคล้องกันทั้ง funnel — งานที่เคยใช้เวลาเดือน ๆ Claude Code ทำได้ในไม่กี่ชั่วโมง
- การเชื่อมต่อ Claude Code เข้า Google Ads ผ่าน Google Ads API + developer token + OAuth (credentials.json) ทำครั้งเดียว (~7 นาที) แล้วสร้างแคมเปญ โฆษณา ad assets negative keywords ได้อัตโนมัติ
- การตั้งค่าสำคัญ: presence only (ไม่ใช้ presence or interest), ตัดประเทศอื่นออก, ปิด auto recommendations และหลีกเลี่ยง performance max (ลีดปลอม/spam จากประสบการณ์จริง $10K/เดือน)
- Speed to lead: โทรภายใน 60 วินาที ทำเงินได้ 4 เท่า (งานวิจัย Velocify) — ใช้ CRM (GoHighLevel) โทรอัตโนมัติภายใน 5-10 วินาทีหลังลีดเข้า พร้อม double dial และแจ้งบน thank you page ว่าจะโทรใน 75 วินาที
- การขาย: นั่งสายนาน 30-60 นาที สร้าง rapport (ทุก 10 นาทีหลังนาทีที่ 20 เพิ่ม conversion 7%), 50% ของยอดขายไปที่คนที่โทรก่อน และควร split test sales script (เพิ่มยอดขาย 15%)
- Analytics: จับคู่ CSV ลีดกับ CRM ด้วยเบอร์โทร เพื่อดูว่า job type/วัน/เวลา/แหล่งลีดไหนทำเงินจริง + ใช้ UTM hidden fields และ Google Click ID เพื่อส่ง offline conversion บอก Google ว่าลูกค้าที่มีกำไรหน้าตาเป็นยังไง
- ปิดท้ายด้วยการ deploy เว็บขึ้น live ผ่าน GitHub + Vercel และสร้าง skills ใน Claude Code เพื่อรันทั้ง workflow ด้วยคำสั่งเดียว เช่น /generate ads

## ความเห็นสรุป

วิดีโอนี้เป็นคู่มือปฏิบัติครบวงจรสำหรับเจ้าของธุรกิจบริการท้องถิ่นที่อยากใช้ Claude Code ลดงาน manual ใน Google Ads ตั้งแต่ตั้งโปรไฟล์จนถึง offline conversion จุดเด่นคือผู้สอนอ้างอิงตัวเลขจริงจากธุรกิจตัวเอง ($180K ค่าโฆษณา → $730K รายได้, $2M ที่ทดสอบ split test) และเตือนภัยของจริง เช่น เมตริกปลอมของ Google และ performance max ที่ได้ลีดขยะ อย่างไรก็ตาม ควรระลึกว่าวิดีโอนี้ยังเป็นช่องทางการตลาดของคอมมูนิตี้แบบเสียเงินของเขาด้วย จึงมีการชวนเข้าร่วมตลอดท้ายวิดีโอ — เนื้อหาหลักยังมีประโยชน์และทำตามได้จริงแม้ไม่สมัครอะไรเลย

