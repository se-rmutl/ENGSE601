# ENGSE601 — การตรวจสอบความสมเหตุสมผลและการทวนสอบซอฟต์แวร์

<p align="center">
  <img src="assets/images/se-rmutl-logo.jpg" alt="SE RMUTL" width="112">
</p>

> **Software Validation and Verification · 3(3-0-6)**  
> หลักสูตรวิศวกรรมศาสตรบัณฑิต สาขาวิชาวิศวกรรมซอฟต์แวร์  
> ชั้นปีที่ 3 · ปีการศึกษา 2569 · มหาวิทยาลัยเทคโนโลยีราชมงคลล้านนา

> **ปรับปรุง 20 ต.ค. 2569** · หน้านี้เขียนใหม่ให้ตรงกับที่เรียนจริงในภาคนี้ · แผนเดิม 17 สัปดาห์ย้ายไปไว้ที่ [`archive/`](archive/README.md)

---

## วันสำคัญ

| วันที่ | เรื่อง |
|---|---|
| **พุธ 21 ต.ค. 2569 10:00–12:00** | สอบปลายภาค take-home รายบุคคล ผ่าน Google Form · ระบบปิดรับ 12:10 · ดู [docs/final-exam.md](docs/final-exam.md) |
| **ศุกร์ 23 ต.ค. 2569 23:59** | ปิดรับงานย้อนหลังทั้งหมด ทั้งงานเดี่ยวและงานกลุ่ม · ดู [docs/deliverables.md](docs/deliverables.md) |

**ไม่มีสอบปากเปล่า**

---

## รายวิชานี้เรียนอะไร

เปลี่ยน “ความต้องการของระบบ” ให้เป็น “หลักฐาน” ที่ตรวจสอบได้ ว่าระบบทำงานถูกต้องตามข้อกำหนด และตอบโจทย์ผู้ใช้

- **Verification** — สร้างถูกตามข้อกำหนดไหม
- **Validation** — สร้างสิ่งที่ผู้ใช้ต้องการจริงไหม
- เริ่มตรวจได้ตั้งแต่ยังไม่มีโค้ด (ตรวจเอกสาร) แล้วค่อยออกแบบและรันการทดสอบ

---

## เส้นทางที่เรียนจริงในภาคนี้

| ช่วง | วันที่ | เรื่อง | กรณีศึกษา | ผลงาน | นับเข้า |
|---|---|---|---|---|---|
| [W01](weeks/week-01-foundation-vv-quality/README.md) | ต้นภาค | คุณภาพและ V&V · Quality Risk Cards | RMUTL Smart Campus | W01 (กลุ่ม) | จิตพิสัย |
| [W02](weeks/week-02-test-process-models/README.md) | ต้นภาค | กระบวนการทดสอบ · Project Quality Route Map | RMUTL Smart Campus | W02 (กลุ่ม) | จิตพิสัย |
| [W03](weeks/week-03-testable-requirements/README.md) | ต้นภาค | ความต้องการที่ทดสอบได้ · Acceptance Criteria | RMUTL Smart Campus | W03 (กลุ่ม) | Gate A |
| [W04](weeks/week-04-requirement-review-traceability/README.md) | ต้นภาค | ทบทวน SRS · RTM Lite · ตัดสิน Gate A | RMUTL Smart Campus | W04 (กลุ่ม) | Gate A |
| สอบกลางภาค | — | Part I รายบุคคล (Variant O/E) | — | ส่งทาง Teams แล้ว | Midterm |
| [W05](weeks/week-05-hld-review-trace/README.md) | 9 ก.ย. | ทบทวนเอกสารออกแบบ (HLD) · Requirement-to-Design Trace | Case X | W05 (กลุ่ม) | Gate B |
| [ครั้งที่ 1](sessions/s1/README.md) | 23 ก.ย. | วางแผนก่อนทดสอบ | Case X | ใบงาน 1 (A เดี่ยว · B กลุ่ม) | ใบงาน A · Evidence Pack |
| [ครั้งที่ 2](sessions/s2/README.md) | 30 ก.ย. | ออกแบบกรณีทดสอบ | Case X Mini | ใบงาน 2 (A เดี่ยว · B กลุ่ม) | ใบงาน A · Evidence Pack |
| [ครั้งที่ 3](sessions/s3/README.md) | 14 ต.ค. | ลงมือทดสอบ (ครั้งสุดท้ายที่สอน) | Case X Mini v0.9 | ใบงานรวม 3–4 (A ข้อ 1–2 · B1 · B3) | ใบงาน A · Evidence Pack |
| ครั้งที่ 4 · W06 | — | **ไม่ได้สอน** · ไม่นับคะแนน | — | — | — |
| สอบปลายภาค | 21 ต.ค. | take-home รายบุคคล | — | Google Form | Final |

รายละเอียดแต่ละครั้งอยู่ใน [`sessions/`](sessions/README.md) · รายละเอียด W01–W05 อยู่ใน [`weeks/`](weeks/)

---

## ลิงก์ที่ใช้บ่อย

| อะไร | ลิงก์ |
|---|---|
| พอร์ทัลเอกสารการสอน (สไลด์ เอกสาร ใบงาน แอปสาธิต) | https://se-rmutl.github.io/engse601/ |
| Template repo ของทีม (กด **Use this template** ตั้งเป็น **Public**) | https://github.com/se-rmutl/engse601-project-template |
| **ตัวอย่างงานกลุ่มที่ทำครบ (Team00 · Case X)** — ใช้ดูรูปแบบ **ห้ามคัดลอกข้อความ** | https://github.com/se-rmutl/ENGSE601-Team00-CaseX-Example |
| เอกสาร Case X: SRS v1.1 | https://se-rmutl.github.io/engse601/materials/casex/ENGSE_CaseX_SRS_v1_1_Practical_TH.docx |
| เอกสาร Case X: HLD v0.9 ฉบับทบทวน | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Draft_for_Review_TH.docx |
| เอกสาร Case X: HLD v0.9 อ่านด้วยภาพ | https://se-rmutl.github.io/engse601/materials/casex/ENGSE601_CaseX_HLD_v0_9_Visual_Guide_TH.html |
| แอปสาธิต Case X Mini v0.9 พร้อมชุดทดสอบ | https://se-rmutl.github.io/engse601/materials/app/CaseXMini_v0.9_Student_S3.zip |
| คู่มือเล่มปริญญานิพนธ์ v3 | https://se-rmutl.github.io/engse601/materials/thesis/ENGSE601_Thesis_Guide_v3.docx |

---

## การประเมินผลโดยสรุป

| คอลัมน์ | % | เดี่ยว/กลุ่ม | มาจากอะไร |
|---|---:|---|---|
| จิตพิสัย | 5 | เดี่ยว | มาเรียน (จาก 8 ครั้ง) คิดเป็น 3 คะแนน + ทีมส่ง W01 ได้ 1 + ทีมส่ง W02 ได้ 1 · **เข้าเรียนต่ำกว่า 80% (มาไม่ถึง 7 ใน 8 ครั้ง) ได้จิตพิสัยครึ่งเดียว** |
| Gate A | 15 | กลุ่ม | W03 (5) + W04 (10) |
| Gate B | 10 | กลุ่ม | W05 (10) |
| สอบกลางภาค | 20 | เดี่ยว | Part I เต็ม 12 แปลงเป็น 20 · Part II ไม่ได้ใช้ |
| ใบงาน A | 10 | เดี่ยว | เฉลี่ยเท่ากัน 3 ใบ: ใบงาน 1 ส่วน A (20) · ใบงาน 2 ส่วน A (30) · ใบงานรวม 3–4 ส่วน A ข้อ 1–2 (14) |
| Evidence Pack | 15 | กลุ่ม | เฉลี่ยเท่ากัน 3 ใบ: ใบงาน 1 ส่วน B (20) · ใบงาน 2 ส่วน B (20) · ใบงานรวม 3–4 ส่วน B1 + B3 (21) |
| สอบปลายภาค | 25 | เดี่ยว | ปรนัย 20 + เขียนตอบ 30 = 50 หารด้วย 2 |
| **รวม** | **100** | | เดี่ยว 60 · กลุ่ม 40 |

- คะแนนรวมปัดเป็นจำนวนเต็มก่อนตัดเกรด (.5 ปัดขึ้น) · A ตั้งแต่ 80 · B+ 75–79 · B 70–74 · C+ 65–69 · C 60–64 · D+ 55–59 · D 50–54 · F ต่ำกว่า 50
- สมาชิกในทีมได้คะแนนกลุ่มเท่ากัน ผู้สอนปรับรายคนได้จาก `TEAM.md` (ใครทำส่วนไหน)
- งานที่ไม่ส่งภายในศุกร์ 23 ต.ค. 2569 23:59 ได้ 0 · ส่งภายในกำหนดนี้ไม่หักคะแนน
- ใบงานรวม 3–4 **ส่วน A ข้อ 3–5** และ **ส่วน B2** ไม่นับคะแนน เพราะไม่ได้สอนครั้งที่ 4
- **ผู้สอนใช้ AI ช่วยตรวจงานเบื้องต้น ผู้สอนเป็นผู้ตัดสินคะแนนสุดท้าย**

รายการงานทั้งหมด ชื่อไฟล์ และที่ส่ง: [docs/deliverables.md](docs/deliverables.md)

---

## กติกาสำคัญ

1. **ผลทดสอบต้องมาจากการรันจริง** ไม่ได้รันให้เขียน `Not Executed` พร้อมเหตุผล · แต่งผลหรือหลักฐาน ส่วนนั้นได้ 0
2. **repo ของทีมเป็น Public** ห้ามใส่รหัสนักศึกษา และห้ามวางงานเดี่ยวส่วน A ใน repo
3. ใช้ AI ช่วยคิดและตรวจทานได้ แต่ต้องตรวจผลเอง และบันทึกใน `AI-LOG.md` · ดู [docs/responsible-ai.md](docs/responsible-ai.md)
4. ตัวอย่าง Team00 ใช้ดูรูปแบบเท่านั้น งานของทีมต้องมาจากงานของทีมเอง

---

## Course Learning Outcomes (CLOs)

| CLO | นักศึกษาสามารถ… |
|---|---|
| **CLO1** | อธิบายหลักการ software quality, testing, verification, validation และแบบจำลองกระบวนการทดสอบได้ |
| **CLO2** | วิเคราะห์ requirements, acceptance criteria, ความเสี่ยง และสร้าง Requirement Review Sheet / Traceability Matrix ได้ |
| **CLO3** | ออกแบบ test strategy, test cases, test data และแนวทางทดสอบในระดับ component, integration, system, UAT และ NFR ได้ |
| **CLO4** | จัดทำ Test Plan ที่มีขอบเขต กลยุทธ์ ความเสี่ยง บทบาท เครื่องมือ และเกณฑ์ติดตามควบคุมได้ |
| **CLO5** | วิเคราะห์ defect, ติดตามผล สรุปผลการทดสอบ และสื่อสารหลักฐาน V&V ได้ |
| **CLO6** | ทำงานร่วมกัน ใช้ AI อย่างรับผิดชอบ ตรวจสอบผลลัพธ์ และเปิดเผยการใช้ AI ได้ |

ภาคนี้ไม่ได้สอนครั้งที่ 4 (รายงานข้อบกพร่องและคำตัดสินส่งมอบ) จึงประเมิน CLO5 ได้น้อย · ดู [docs/clo-plo-assessment.md](docs/clo-plo-assessment.md)

---

## โครงสร้าง Repository

```text
ENGSE601/
├── README.md             # หน้านี้
├── docs/                 # คู่มือรายวิชา งานที่ต้องส่ง สอบปลายภาค CLO/PLO และ AI
├── sessions/             # ครั้งที่ 1–3 (ชุด 4 ครั้งสุดท้าย ไม่ได้สอนครั้งที่ 4)
├── weeks/                # W01–W05
├── templates/            # แบบฟอร์มเดิม (งานที่ส่งจริงใช้ template repo ของทีม)
├── archive/              # แผนเดิม 17 สัปดาห์ ไม่ได้ใช้ในภาคนี้
├── assets/images/        # ตราสัญลักษณ์
└── .github/              # issue / pull request templates
```

---

## ผู้รับผิดชอบรายวิชา

**อาจารย์ธนิต เกตุแก้ว**  
สาขาวิชาวิศวกรรมซอฟต์แวร์ คณะวิศวกรรมศาสตร์  
มหาวิทยาลัยเทคโนโลยีราชมงคลล้านนา
