

# 🏦 Online Banking REST API (Spring Boot)

A backend REST API for a simple online banking system built with **Java Spring Boot**, designed to handle user authentication, bank accounts, transactions, and payments. The API uses **JWT tokens** for secure authentication and supports common banking workflows like deposits, withdrawals, transfers, and viewing account history. ([GitHub][1])
<img width="1904" height="958" alt="loginPage" src="https://github.com/user-attachments/assets/8b354a6d-cc87-45b0-8adc-891ca528d4ab" />
<img width="1900" height="931" alt="ProjecPage1" src="https://github.com/user-attachments/assets/7eefd6f8-7ed4-4f1c-80f9-7e622065b4a9" />
<img width="1823" height="895" alt="ProjectPage2" src="https://github.com/user-attachments/assets/5f953abe-461a-46ba-9b63-d99e9dca739c" />
<img width="1902" height="843" alt="ProjectPage3" src="https://github.com/user-attachments/assets/7324d943-464f-457d-966d-fe884386bf54" />
<img width="1894" height="923" alt="ProjectPage5" src="https://github.com/user-attachments/assets/4b671f92-5447-4f39-a7e9-ec59f4abff64" />

---

## 🚀 Features

✔ User registration and login
✔ JWT-based authentication & authorization
✔ Create and manage bank accounts
✔ Perform transactions (deposit, withdraw, transfer)
✔ Make payments
✔ View account balances and histories
✔ Clean structure following **SOLID principles** and design patterns
✔ Tested via **Postman**
✔ MySQL as the database backend ([GitHub][1])

---

## 📦 Technologies

* **Java 17+**
* **Spring Boot**
* **Spring Security (JWT)**
* **MySQL**
* **Postman (for testing)**
* **Maven (build tool)**
* **Dockerfile included** ([GitHub][1])

---

## 📌 API Endpoints

### 🔐 Authentication

| Endpoint    | Method | Description                   |
| ----------- | ------ | ----------------------------- |
| `/register` | POST   | Register a new user           |
| `/login`    | POST   | User login; returns JWT token |

---

### 🏦 Accounts

| Endpoint                  | Method | Description                    |
| ------------------------- | ------ | ------------------------------ |
| `/app/dashboard`          | GET    | View all accounts and balances |
| `/account/create_account` | POST   | Open a new bank account        |

---

### 💸 Transactions

| Endpoint                   | Method | Description               |
| -------------------------- | ------ | ------------------------- |
| `/transact/deposit`        | POST   | Deposit funds             |
| `/transact/withdraw`       | POST   | Withdraw funds            |
| `/transact/transfer`       | POST   | Transfer between accounts |
| `/app/payment_history`     | GET    | View payment history      |
| `/app/transaction_history` | GET    | View transaction history  |

---

## 🧪 How to Use (Quickstart)

1. **Clone the repo**

   ```bash
   git clone https://github.com/AnnaGH-hub/Project-S5.git
   cd Project-S5
   ```

2. **Configure the database**

   * Create a MySQL database
   * Update `application.properties` with your DB credentials

3. **Build and run**

   ```bash
   mvn clean install
   mvn spring-boot:run
   ```

4. **Test with Postman**

   * Import the Postman collection (if included)
   * Test signup, login, then use the returned JWT token to access protected routes

---

## 🧠 Notes & Design

* The project strictly follows **SOLID principles** and common design patterns for maintainability. 
* Uses **JWT + Interceptors** for secure session handling. 
---

