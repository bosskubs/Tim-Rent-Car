# Tim Rent Car (Group Project)

## Project Overview
Tim Rent Car เป็นโครงการออกแบบและพัฒนาระบบบริหารจัดการเช่ารถ (Academic Car Rental Management System) ซึ่งครอบคลุมระบบการค้นหารถ, การจอง, การตรวจสอบเวลาทับซ้อน, การรับคืนรถ, และการตรวจสภาพ 

*(หมายเหตุ: Source Code และ Web Prototype ภายใน Repository นี้ ถูกพัฒนาขึ้นโดยใช้ JavaScript/Node.js และ SQLite เป็นหลักสำหรับการสาธิตฟังก์ชันเบื้องต้น โดยเพื่อนร่วมกลุ่มรับผิดชอบส่วนของ Development)*

## System Architecture & Features
* Backend: Node.js (v24+) 
* Database: SQLite (พร้อมระบบ Backup อัตโนมัติทุกชั่วโมง)
* Key Workflows: 
  * ระบบจองและเช็คช่วงเวลาทับซ้อน
  * ระบบ Roles & Permissions 4 ระดับ (Customer, Staff, Admin, Inspector)
  * ระบบจำลองการชำระเงินและแจ้งเตือนผ่าน Test Inbox
  * ระบบสร้างและดาวน์โหลดเอกสารสัญญา/ใบเสร็จเป็น PDF (ภาษาไทย)

## My Contribution (System Analysis & Design)
ในโครงการกลุ่มนี้ ผมรับผิดชอบในส่วนของการวิเคราะห์และออกแบบระบบ (System Analysis):
* **Use Case Diagram (UML):** ออกแบบ Use Case Diagram เพื่อกำหนดขอบเขตของระบบ (System Boundary) และระบุความสัมพันธ์ระหว่างผู้ใช้งาน (Actors) กับฟังก์ชันการทำงานต่างๆ
* **Role & Permission Analysis:** วิเคราะห์และกำหนดสิทธิ์การเข้าถึงระบบของ Actor ระดับต่างๆ เช่น เจ้าหน้าที่บริการ (Staff), ผู้ดูแลระบบ (Admin) และ เจ้าหน้าที่ตรวจสอบสภาพรถ (Inspector)
* **System Workflow:** ออกแบบฟังก์ชันการทำงานของระบบตาม Requirement เช่น การจองรถ, การจัดการข้อมูลลูกค้า, การเชื่อมต่อระบบชำระเงินผ่าน API (QR/Credit Card), และการบันทึกประวัติการซ่อมบำรุง
