# 📚 Library Management System

This **Library Management System** is a C++/SQL-based application designed to manage books, members, staff, borrow transactions, and reservations efficiently.  
The system provides features such as fine calculation, overdue tracking, book availability, and persistent data handling for a realistic library management workflow.

It was developed as part of Computer Engineering coursework to strengthen database management, SQL querying, and system design skills.

---

## 🎯 Project Objectives

The main goals of this system are:

- Manage **books, authors, categories, publishers, members, and staff** efficiently  
- Track **borrow transactions**, fines, and overdue books  
- Handle **reservations** and book availability  
- Ensure **data consistency** across all operations  
- Practice **SQL queries, joins, aggregation, and advanced data handling**  

---

## ⚙️ System Overview

The system allows librarians and staff to:

1. Add, update, and remove books, members, and staff  
2. Record borrow transactions and calculate fines  
3. Track overdue books and reservations  
4. Generate reports on fines, active users, and staff activity  
5. Maintain strong data consistency across all operations  

---

## 🚀 Features

- ✅ Delete borrow transactions with zero fine and already returned  
- ✅ Update book copies availability  
- ✅ List members with overdue books  
- ✅ Calculate total fines collected and top members by fines  
- ✅ Count borrow transactions handled by each staff  
- ✅ Show books currently borrowed  
- ✅ Display members with fines above average  
- ✅ Show reservation statistics by status  
- ✅ Track last borrow date for each member  
- ✅ List reserved books not yet borrowed  
- ✅ Handle missing contact info for members  
- ✅ Categorize books by availability  
- ✅ Display staff role even if missing  
- ✅ Identify active members and those who borrowed AND reserved books  
- ✅ Calculate months since members joined  
- ✅ Show remainder of fines and overdue durations (days, weeks, months)  

---

## 🛠 Technologies Used

- **Database:** PostgreSQL / MySQL (SQL queries and table management)  
- **Programming Language:** C++ / SQL (depending on implementation)  
- **Concepts:** Relational database design, joins, aggregate functions, foreign keys, constraints  
- **Tools:** Git, GitHub, VS Code / IntelliJ / DBeaver / pgAdmin  

---

## 🧩 Database Design

The system uses the following tables and relationships:

- **Authors, Categories, Publishers:** Store metadata for books  
- **Books:** Core entity with copies availability and ISBN  
- **Members & Staff:** User and staff data management  
- **BorrowTransactions / Borrows:** Track book loans and fines  
- **Reservations / Reserves:** Manage pending or completed reservations  
- **Relationship Tables:** Handle 1-to-many and many-to-many associations  
  - Writes (Author → Book)  
  - Publishes (Publisher → Book)  
  - BelongsTo (Book → Category)  
  - Handles (Staff → BorrowTransactions)  

---

## 🗂 Entity-Relationship Diagram (ERD)

The following ERD illustrates the relationships between all tables in the Library Management System:

![Library ERD](images/ERD.png)

> Place your ERD image in the `images/` folder and name it `ERD.png` for this to display correctly.

---

## 📁 Project Structure

Organizing the repository like a professional project:
library-management-system/
│
├── sql/ → All SQL scripts (CREATE TABLE, INSERT, queries)
├── data/ → Sample CSV/JSON datasets (if any)
├── images/ → ERD and other visuals
└── README.md → Project documentation

**Why this structure matters:**

- ✅ Keeps SQL scripts separate from source code  
- ✅ Provides folders for data and documentation  
- ✅ Shows recruiters you understand modular project organization  
- ✅ Makes the project maintainable and scalable  

