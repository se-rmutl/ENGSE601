# ครั้งที่ 1 วางแผนก่อนทดสอบ

**วันที่:** พุธ 23 ก.ย. 2569 · **กรณีศึกษา:** Case X (SRS v1.1 · HLD v0.9)  
**คำถามหลัก:** กฎอยู่ส่วนประกอบไหน และทดสอบอะไรก่อน

## เป้าหมาย

ยังไม่มีโค้ด ก็ทดสอบเอกสารได้แล้ว ครั้งนี้ทบทวนเอกสารออกแบบของ Case X แล้วเขียนแผนทดสอบฉบับย่อ

หลังเรียนต้องทำได้:

1. จับคู่ขั้นการพัฒนากับระดับการทดสอบบน V-Model
2. ทบทวนเอกสารออกแบบด้วย 3 คำถาม และเขียนข้อค้นพบที่นำไปแก้ได้
3. เขียนแผนทดสอบย่อ จัดลำดับความเสี่ยง และแยก Entry/Exit ที่วัดได้

## แนวคิดสำคัญ

- **V-Model** แต่ละขั้นทางซ้าย (ความต้องการ · ออกแบบ · รายละเอียด) เป็นฐานการทดสอบของระดับทางขวา
- **การทบทวนแบบสถิต** หาข้อบกพร่องในเอกสารได้ก่อนเขียนโค้ด แก้ง่ายและถูกกว่า
- **ตำแหน่งของกฎ** หาว่ากฎแต่ละข้อถูกตรวจที่ส่วนประกอบใดในเอกสารออกแบบ ผลนี้ใช้ต่อในครั้งที่ 2 และ 3
- **ข้อค้นพบ** เขียนให้ครบ 4 ส่วน หรือมีหลักฐานว่าตรวจแล้วไม่พบปัญหา
- **แผนทดสอบย่อ** ขอบเขต · สิ่งที่ไม่ทดสอบพร้อมเหตุผล · ระดับ · ลำดับความเสี่ยง · สภาพแวดล้อม
- **Entry / Exit** Entry = ต้องพร้อมอะไรก่อนเริ่มทดสอบ · Exit = เมื่อไรจึงถือว่าทดสอบเสร็จ · ต้องวัดได้

## เอกสาร (พอร์ทัล)

| เอกสาร | ลิงก์ |
|---|---|
| หน้าครั้งที่ 1 | https://se-rmutl.github.io/engse601/sessions/s1.html |
| เอกสารประกอบการสอน | https://se-rmutl.github.io/engse601/materials/s1/ENGSE601_S1_Teaching_Doc_TH.html |
| สไลด์ | https://se-rmutl.github.io/engse601/materials/s1/ENGSE601_S1_Slides_TH.html |
| ใบงานครั้งที่ 1 | https://se-rmutl.github.io/engse601/materials/s1/ENGSE601_S1_Worksheet_TH.docx |
| แนวทางการทำใบงาน | https://se-rmutl.github.io/engse601/materials/s1/ENGSE601_S1_Worksheet_Guide_TH.html |
| ดาวน์โหลดทั้งชุด | https://se-rmutl.github.io/engse601/materials/s1/ENGSE601_S1_Student_Pack.zip |
| CaseX SRS v1.1 | https://se-rmutl.github.io/engse601/materials/casex/ENGSE_CaseX_SRS_v1_1_Practical_TH.docx |
| CaseX HLD v0.9 ฉบับทบทวน | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Draft_for_Review_TH.docx |
| CaseX HLD v0.9 อ่านด้วยภาพ | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Visual_Guide_TH.html |

## ส่งอะไร

| ส่วน | ใคร | ส่งที่ไหน | ชื่อไฟล์ | เต็ม | นับเข้า |
|---|---|---|---|---:|---|
| ใบงานทั้งฉบับ (A + B) | ทุกคน | Google Form ส่งงานเดี่ยว | `S1_<รหัสนักศึกษา>.pdf` (ระบบตั้งให้) | A 20 | ใบงาน A |
| ส่วน B เท่านั้น | ทีม | repo ของทีม | `01-plan/S1-B_<TeamName>.pdf` | 20 | Evidence Pack |

- ใน repo วาง **เฉพาะส่วน B** ห้ามมีส่วน A ของใคร
- ปิดรับ **ศุกร์ 23 ต.ค. 2569 23:59**
