# Report 1: Project Description Report

**Course:** Data Science / UML Modelling
**Institution:** Université Libre de Kigali (ULK)
**Instructor:** Eric Maniraguha
**Team Members:** [Mohamed Tarig Ahmed Taha][202513604] and [Student Name 2]
**Date:** October 2026

---

## 1. Project Title

**Hotel Booking System: Design of a UML Class Diagram**

## 2. Business Idea

The business idea is to provide a centralised software system that helps a hotel manage the core of its daily operations: who its guests are, which rooms it has, who has reserved which room and when, and whether those reservations have been paid for.

Instead of relying on paper registers or scattered spreadsheets, the hotel would use one consistent model of its data. Every booking is tied to a registered guest and a specific room, and every payment is tied to the booking it settles. This gives the hotel a reliable record and gives guests a smoother reservation experience.

## 3. Problem Statement

Hotels that manage reservations manually face several recurring problems:

1. **Double bookings.** Without a central record, the same room can be promised to two guests for overlapping dates.
2. **Scattered or lost guest information.** Guest details kept in different places are hard to find, update or keep accurate.
3. **Unclear room status.** Staff cannot quickly tell which rooms are available, occupied or under maintenance.
4. **Untraceable payments.** It is difficult to confirm whether a given booking has been paid, partially paid or refunded.
5. **Slow and error-prone processes.** Manual calculation of totals and manual record keeping take time and invite mistakes.

## 4. Purpose of the Proposed System

The purpose of the Hotel Booking System is to:

- provide a clear and well-structured **model** of the hotel's core entities and how they relate,
- support **accurate guest registration** and record keeping,
- allow **efficient room management** and availability checking,
- enable **conflict-free booking reservations**,
- keep a **traceable record of payments** for each booking,
- serve as a solid foundation that developers can use to later implement the system in code and a database.

For this course assignment, the specific purpose is to demonstrate the ability to analyse a real-world scenario and express it as a UML Class Diagram with correct classes, attributes, operations, relationships and multiplicities.

## 5. Project Scope

### 5.1 Functions Covered

| # | Function | Description |
|---|---|---|
| 1 | Guest registration | Register new guests, store and update their personal and contact details. |
| 2 | Room management | Add rooms, define type and price, check availability and update status. |
| 3 | Booking reservations | Create, change and cancel bookings; calculate the total cost of a stay. |
| 4 | Payment processing | Record payments, track payment status, record refunds and generate receipts within the system. |

### 5.2 Functions Excluded

| # | Excluded item | Explanation |
|---|---|---|
| 1 | Third-party live credit card gateways | The system records payments internally but does not connect to external card processors. |
| 2 | Staff payroll | Salary, attendance and HR management are outside this project. |
| 3 | Physical inventory | Management of physical stock such as linens, food and supplies is not included. |

## 6. System Requirements

### 6.1 Functional Requirements

| ID | Requirement |
|---|---|
| FR1 | The system shall allow a new guest to register with personal and contact details. |
| FR2 | The system shall allow guest information to be updated. |
| FR3 | The system shall allow rooms to be added with a number, type, price and capacity. |
| FR4 | The system shall allow room status to be updated (for example available, booked, maintenance). |
| FR5 | The system shall check whether a room is available for a requested date range. |
| FR6 | The system shall allow a registered guest to book an available room. |
| FR7 | The system shall calculate the total cost of a booking from the number of nights and the room price. |
| FR8 | The system shall allow a booking to be cancelled and its status updated. |
| FR9 | The system shall record a payment for a booking, including amount, date and method. |
| FR10 | The system shall track payment status and allow a receipt to be generated. |

### 6.2 Non-Functional Requirements

| ID | Requirement |
|---|---|
| NFR1 | **Usability:** the system should be simple enough for hotel staff with basic computer skills. |
| NFR2 | **Data integrity:** every booking must reference a valid guest and a valid room. |
| NFR3 | **Reliability:** the system should prevent overlapping bookings of the same room. |
| NFR4 | **Maintainability:** the design should be modular so that classes can be extended later. |
| NFR5 | **Security:** guest personal data should be accessible only to authorised users. |

### 6.3 Design Assumptions

- Each booking is for **one room**; a guest who needs several rooms makes several bookings.
- Each booking is settled by **one payment record** (a simplification for this assignment).
- A room can be booked many times, but never for overlapping dates.

## 7. Conclusion

The Hotel Booking System addresses common weaknesses of manual hotel record keeping by modelling four core classes (Guest, Room, Booking and Payment) and the relationships between them. Report 2 presents the detailed UML Class Diagram that translates this description into a formal design.
