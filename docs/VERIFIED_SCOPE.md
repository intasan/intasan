# ขอบเขตที่ตรวจสอบจากระบบจริง

Repository: `intasan/intasan`
ฐาน source ที่ตรวจ: `b875e7f280c4b1062b4043c7a4550b7a58c2feaf`

**สถานะ: ตรวจ source โปรไฟล์**

README เป็น landing page; ใช้สถานะจาก evidence ของแต่ละ Repository เท่านั้น

## แหล่งหลักฐาน

- [evidence/source-audit.json](../evidence/source-audit.json)

## Traceability จาก source

| ไฟล์ที่ตรวจ | ขอบเขตที่ยืนยันได้ |
|---|---|

## เกณฑ์ตรวจรับ BA / SA

| เกณฑ์ | หลักฐาน / สถานะ |
|---|---|
| ขอบเขตปัจจุบันตรงกับ source | ตรวจ source โปรไฟล์ |
| End-to-end ด้วยข้อมูลจริง | README เป็น landing page; ใช้สถานะจาก evidence ของแต่ละ Repository เท่านั้น |
| ผลการทดสอบที่ทำซ้ำได้ | อ่าน command, stdout, exit code ใน evidence; syntax check ไม่ใช่ runtime test |
| ข้อมูลจริงและ provenance | เฉพาะราคาทองใน live-verification.txt ที่มี URL/เวลา publication; ไม่ใช้ fixture เป็นข้อมูลจริง |
| UAT โดยเจ้าของงานหรือผู้ใช้งาน | ยังไม่ได้ดำเนินการในรอบนี้ |

## ข้อจำกัดการแสดงผลงาน

ผล unit tests เป็นการตรวจ logic โดยมี fixture ตาม suite เดิม ไม่ใช่หลักฐานธุรกรรมจริง การฝึกโมเดลจริง การทำงานของอุปกรณ์จริง หรือการรับรองจากผู้ใช้ ไม่สร้างข้อมูลธุรกิจทดแทนข้อมูลที่ขาด และไม่อนุมานว่าไม่มีข้อมูลเท่ากับปลอดภัย
