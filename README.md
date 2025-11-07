# Java-mini-project
# 🗳️ Online Voting System (Java Project)

![Java](https://img.shields.io/badge/Java-17-orange?style=for-the-badge)
![MySQL](https://img.shields.io/badge/MySQL-Database-blue?style=for-the-badge)
![JavaFX](https://img.shields.io/badge/JavaFX-GUI-green?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)

---

## 📖 Overview
The **Online Voting System** is a Java-based mini project designed to simulate a **secure, digital voting process**.  
It enables users to register, log in, and cast their votes electronically, while the admin can view and manage results.  
This project demonstrates Java concepts such as **OOP, Exception Handling, File Handling, Multithreading, JDBC**, and **JavaFX GUI** — each implemented as a separate module.

---

## 🧩 Project Modules

| Module | File | Concept | Description |
|:--:|:--|:--|:--|
| 1 | `mod1.java` | Java Basics & OOP | Handles voter registration and validation using object-oriented principles. |
| 2 | `mod2.java` | Exception Handling & Streams | Manages candidate data with file I/O and custom exceptions. |
| 3 | `mod3.java` | Generics & Multithreading | Simulates voting using concurrent threads and generics for flexibility. |
| 4 | `mod4.java` | JDBC & Database Connectivity | Connects to MySQL to fetch and update candidate details dynamically. |
| 5 | `mod5.java` | JavaFX GUI Integration | Provides a graphical interface for login and vote casting. |

---
🧱 System Architecture
      ┌────────────────────────┐
      │        USER (Voter)    │
      └────────────┬───────────┘
                   │
                   ▼
       ┌──────────────────────────┐
       │   JavaFX Login Interface  │
       └────────────┬─────────────┘
                   │
                   ▼
       ┌──────────────────────────┐
       │  Backend Logic (Java)    │
       │  - Registration          │
       │  - Authentication        │
       │  - Vote Casting          │
       └────────────┬─────────────┘
                   │
                   ▼
       ┌──────────────────────────┐
       │   MySQL Database          │
       │   - Candidates Table      │
       │   - Votes Count           │
       └────────────┬─────────────┘
                   │
                   ▼
       ┌──────────────────────────┐
       │   Admin / Result Viewer   │
       └──────────────────────────┘
       
---

## ⚙️ Technologies Used
- ☕ **Java (JDK 17 or later)**
- 🧩 **JavaFX** – for GUI interface
- 🗄️ **JDBC** – for database connectivity
- 💾 **MySQL** – for data storage
- 💻 **IDE** – NetBeans / IntelliJ / Eclipse

---
 🗂️ Folder Structure

---

🗃️ Database Setup
1. Open MySQL and create a database:
   
CREATE DATABASE votingdb;
USE votingdb;
CREATE TABLE candidates (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    party VARCHAR(100),
    votes INT DEFAULT 0
);
insert into candidates values
(1,"devesh", "ASL", 50000),
(2,"chanak","CVK",60000),
(3,"Buvanesh","MMK",70000);


