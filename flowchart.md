```mermaid
usecaseDiagram
    actor Admin as "ผู้ดูแลระบบ (Admin)"

    rectangle "ระบบจัดเก็บข้อมูลครุภัณฑ์" {
        usecase "เข้าสู่ระบบ (Login)" as UC1
        usecase "ดูภาพรวมระบบ (View Dashboard)" as UC2
        usecase "ค้นหาและจัดการครุภัณฑ์ (Manage Assets)" as UC3
        usecase "จัดการประเภทและสถานที่ (Manage Master Data)" as UC4
        usecase "แจ้งปัญหา/แจ้งซ่อม (Report Issue)" as UC5
        usecase "ตรวจสอบครุภัณฑ์ (Inspect Asset)" as UC6
        usecase "ดูประวัติการดำเนินงาน (View History)" as UC7
        usecase "ตั้งค่าการแจ้งเตือน (Manage Notifications)" as UC8
        usecase "จัดการผู้ใช้งาน (Manage Users)" as UC9
    }

    Admin --> UC1
    Admin --> UC2
    Admin --> UC3
    Admin --> UC4
    Admin --> UC5
    Admin --> UC6
    Admin --> UC7
    Admin --> UC8
    Admin --> UC9

    UC2 ..> UC1 : <<include>>
    UC3 ..> UC1 : <<include>>
    UC4 ..> UC1 : <<include>>
    UC5 ..> UC1 : <<include>>
    UC6 ..> UC1 : <<include>>
    UC7 ..> UC1 : <<include>>
    UC8 ..> UC1 : <<include>>
    UC9 ..> UC1 : <<include>>
```
