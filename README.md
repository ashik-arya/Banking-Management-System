# 💰 Banking Management System

A console-based **Banking Management System** developed using **Java** and **MySQL**, designed to handle essential banking operations like user authentication, balance management, deposits, and withdrawals.

---

## 🚀 Features

- 🔐 User login using account number and password  
- 🏦 View and manage account details  
- 💸 Deposit and withdraw funds  
- 📊 Real-time balance tracking  
- 🔁 Secure transactions with security PIN  
- 🗃️ MySQL database integration using JDBC  
- 📌 Clean object-oriented structure

---

## 🛠️ Tech Stack

- Java (Core Java)
- MySQL
- JDBC (Java Database Connectivity)
- Console-based Interface

---

## 🗃️ Database Schema

### 👤 Table: `users`

Used for authenticating users with account number and password.

| Column           | Type           | Description                       |
|------------------|----------------|-----------------------------------|
| `account_number` | BIGINT (PK)    | Unique account number             |
| `email`          | VARCHAR(100)   | User email (must be unique)       |
| `password`       | VARCHAR(100)   | Login password                    |



🏦 Table: accounts
Stores bank account details associated with users.

| Column           | Type          | Description                     |
| ---------------- | ------------- | ------------------------------- |
| `account_number` | BIGINT (PK)   | Same as in `users` (FK)         |
| `full_name`      | VARCHAR(100)  | Account holder’s full name      |
| `email`          | VARCHAR(100)  | Linked user email               |
| `balance`        | DECIMAL(10,2) | Current account balance         |
| `security_pin`   | VARCHAR(10)   | Used for transaction validation |






