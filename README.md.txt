# Practo Healthcare Database Schema

This project models a scalable healthcare platform database inspired by Practo.

## 🏥 Project Overview

The database supports:

- Patient management
- Doctor management
- Clinic operations
- Appointment booking
- Teleconsultations
- Prescriptions
- Payments

The schema is designed using normalization principles (up to 3NF) and supports scalable healthcare workloads.

---

## 📊 Entity Relationship Model

![ERD](ERD.png)

### Core Relationships

- Patient (1) → (M) Appointments
- Doctor (1) → (M) Appointments
- Clinic (1) → (M) Appointments
- Appointment (1) → (1) Consultation
- Consultation (1) → (M) Prescriptions
- Appointment (1) → (1) Payment

---

## 🗄 Database Design Features

- Primary & Foreign Key constraints
- CHECK constraints
- Indexed high-query columns
- 3NF Normalization
- Suitable for OLTP healthcare systems

---

## 🚀 How to Run

1. Create database in PostgreSQL
2. Run `schema.sql`
3. Generate ERD via pgAdmin

---

## 💡 Concepts Demonstrated

- Schema Design
- ER Modeling
- Normalization (1NF–3NF)
- ACID compliance
- Indexing
- Healthcare data modeling