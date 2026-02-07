# University-Asset-Management System Flowchart

```mermaid
flowchart TD
    Start([เริ่มต้น])
    Login["Admin Login"]
    Firebase["ตรวจสอบตัวตนด้วย Firebase"]
    Decision{เข้าสู่ระบบสำเร็จ?}
    Error["แสดงข้อความผิดพลาด"]
    End1([สิ้นสุด])
    Dashboard["แสดง Dashboard"]
    Manage["จัดการข้อมูลครุภัณฑ์"]
    ReadWrite["บันทึก / อ่านข้อมูล"]
    Firestore[("Cloud Firestore")]
    Display["แสดงผลข้อมูล"]
    End2([สิ้นสุด])
    
    Start --> Login
    Login --> Firebase
    Firebase --> Decision
    Decision -->|ไม่| Error
    Error --> End1
    Decision -->|ใช่| Dashboard
    Dashboard --> Manage
    Manage --> ReadWrite
    ReadWrite --> Firestore
    Firestore --> Display
    Display --> End2
    
    style Start fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style End1 fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style End2 fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Login fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Firebase fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Decision fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Error fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Dashboard fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Manage fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style ReadWrite fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Firestore fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
    style Display fill:#ffffff,stroke:#000000,stroke-width:2px,color:#000000
```
