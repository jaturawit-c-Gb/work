```mermaid
usecaseDiagram
    actor Admin
    rectangle "Durable Goods Management System" {
        usecase "Login" as UC1
        usecase "View Dashboard" as UC2
        usecase "Manage Assets" as UC3
        usecase "Manage Master Data" as UC4
        usecase "Report Issue" as UC5
        usecase "Inspect Asset" as UC6
        usecase "View History" as UC7
        usecase "Manage Notifications" as UC8
        usecase "Manage Users" as UC9
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

    UC2 ..> UC1 : include
    UC3 ..> UC1 : include
    UC4 ..> UC1 : include
    UC5 ..> UC1 : include
    UC6 ..> UC1 : include
    UC7 ..> UC1 : include
    UC8 ..> UC1 : include
    UC9 ..> UC1 : include
```
