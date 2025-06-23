# Library Management System – Database Schema Design

## Objective
Design and implement a relational database schema for a **Library Management System**. This project includes table creation, relationship definition, and an ER diagram.

---

## Tools & Technologies Used

- **MySQL** – for database and SQL execution
- **MySQL Workbench** – to write and execute SQL queries
- **Visual Studio Code (VS Code)** – for editing and saving SQL scripts
- **dbdiagram.io** – to create the Entity Relationship (ER) Diagram

---

## Database Overview

The system includes four main entities:

1. **Author** – stores author information
2. **Book** – stores book details and links to the author
3. **Member** – stores library member information
4. **Borrow** – records which member borrowed which book, and when

---

## Database Schema

### Tables Created:
- `Author(AuthorID, Name)`
- `Book(BookID, Title, Genre, AuthorID)`
- `Member(MemberID, Name, Email, Phone)`
- `Borrow(BorrowID, MemberID, BookID, BorrowDate, ReturnDate)`

### Relationships:
- One Author can write many Books
- One Member can borrow many Books
- One Book can be borrowed by many Members (over time)

---

## Files Included

| File Name              | Description                                 |
|------------------------|---------------------------------------------|
| `library_schema.sql`   | SQL script to create the database and tables |
| `library_er_diagram.png` | ER diagram showing entities & relationships |
| `README.md`            | Project documentation                       |

---

## How to Run

1. Open **MySQL Workbench**
2. Run the `library_schema.sql` file to create the database
3. View ER Diagram using the `library_er_diagram.png` file

---

## Author table desc
![image](https://github.com/user-attachments/assets/1c800aa8-5023-4e3a-b364-1c2b44fd8f6f)

## Book table desc
![image](https://github.com/user-attachments/assets/d9c0c6b2-11c7-49b1-90aa-ae6986807633)

## Member table desc
![image](https://github.com/user-attachments/assets/fd1f9e14-6ce6-4a89-9f36-910ab8d2d8c7)

## Borrow table desc
![image](https://github.com/user-attachments/assets/282c981b-404e-433e-a882-8416d277eeec)

---

## Author

- **Anjana B. Nair**
- Tools: MySQL Workbench, dbdiagram.io, VS Code

---
