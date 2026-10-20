# สัปดาห์ที่ 5 — ทบทวนเอกสารออกแบบ (HLD) และ Requirement-to-Design Trace

> **ภาคการศึกษา 2569** · เรียนพุธ 9 ก.ย. 2569 · กรณีศึกษา **Case X — Multi-Resource Event Booking**  
> งานกลุ่ม **W05 Requirement-to-Design Trace** · นับเข้า **Gate B (10 คะแนน)**  
> ส่งภายใน **ศุกร์ 23 ต.ค. 2569 23:59** · ดู [docs/deliverables.md](../../docs/deliverables.md)  
> หน้านี้ใช้แทนหน้าเดิมที่เขียนว่า Component/Unit Testing ซึ่งไม่ได้สอน

## สัปดาห์นี้ทำอะไร

ตรวจว่า **เอกสารออกแบบรองรับความต้องการหรือไม่** ก่อนเขียนโค้ดบรรทัดแรก

คำถามหลัก: *ความต้องการข้อนี้ มีส่วนประกอบใดรับผิดชอบ และถ้าพฤติกรรมนั้นผิด เราจะเห็นได้ที่จุดใด*

**สัปดาห์นี้ยังไม่มีการทดสอบ** ห้ามมีคำว่า Pass หรือ Fail ในงานที่ส่ง

## เอกสารที่ใช้ (พอร์ทัล)

| เอกสาร | ใช้ทำอะไร | ลิงก์ |
|---|---|---|
| CaseX SRS | ความต้องการต้นทาง | https://se-rmutl.github.io/engse601/materials/casex/ENGSE_CaseX_SRS_v1_1_Practical_TH.docx |
| CaseX HLD v0.9 ฉบับทบทวน | เอกสารออกแบบที่ทบทวน (ฉบับร่าง ไม่ใช่คำตอบที่ถูก) | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Draft_for_Review_TH.docx |
| CaseX HLD v0.9 อ่านด้วยภาพ | อ่านโครงสร้างส่วนประกอบได้เร็ว | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Visual_Guide_TH.html |

ถ้าใบงานของสัปดาห์ระบุรุ่นของ SRS ไว้ ให้อ้างรุ่นตามที่ใช้จริงในงานของทีม

## แนวคิดสำคัญ

- **Trace** โยงความต้องการ → ส่วนประกอบที่รับผิดชอบ → จุดที่สังเกตผลได้
- **สถานะการรองรับ** `Supported` · `Partially Supported` · `Not Supported` · `Not Verifiable` · ตัดสินตามที่เอกสารเขียนจริง
- **ข้อค้นพบ** แยก Fact (เอกสารเขียนไว้) · Inference (เราอนุมาน) · Missing Evidence (เอกสารไม่ได้บอก)
- **ความเสี่ยงเชิงออกแบบ** บอกผลกระทบต่อการทดสอบได้
- **คำถามที่ต้องยืนยัน** มีผู้ตอบและกำหนดเวลา
- ผลของสัปดาห์นี้ (กฎอยู่ส่วนประกอบไหน) ใช้ต่อในครั้งที่ 1

## ส่งอะไร

| งาน | ไฟล์และตำแหน่งใน repo ของทีม |
|---|---|
| W05 Requirement-to-Design Trace | `WEEKS/week-05/submission/W05_<TeamName>_Requirement-to-Design-Trace_v1.pdf` |

ขั้นตอน รหัสที่ใช้ (TR · HF · DR · DQ) ไฟล์ work และเกณฑ์ 10 คะแนน อยู่ใน `WEEKS/week-05/README.md` ของ template repo:
https://github.com/se-rmutl/engse601-project-template/tree/main/WEEKS/week-05

ตัวอย่างงานที่ทำครบ (ใช้ดูรูปแบบ ห้ามคัดลอกข้อความ): https://github.com/se-rmutl/ENGSE601-Team00-CaseX-Example

## การใช้ AI

ใช้ช่วยตั้งคำถามกับเอกสารหรือเรียบเรียงถ้อยคำได้ แต่ **ห้ามให้ AI ตัดสินว่าส่วนประกอบใดรับผิดชอบ หรือเติมส่วนประกอบที่ไม่มีในเอกสาร** · บันทึกใน `AI-LOG.md`
