# 💰 Personal Finance Manager

A full-featured Spring Boot web application designed to help users manage their personal finances by tracking incomes, expenses, savings goals, and generating analytical reports.

[![Java](https://img.shields.io/badge/Java-17+-blue.svg)](https://openjdk.org/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![Docker](https://img.shields.io/badge/Deployed-Docker-blue)](https://www.docker.com/)
[![Render](https://img.shields.io/badge/Live_Render-Available-green)](https://personal-finance-manager-9ja1.onrender.com)

---

## 🚀 Live Demo

🔗 **Deployed API**: https://personal-finance-manager-9ja1.onrender.com

---

## 📸 Preview

![Finance Manager Dashboard](assets/finance_manager_dashboard.png)
![Screenshot 2025-06-14 213203](https://github.com/user-attachments/assets/f893bd38-67a1-40e6-89f0-57dbf3f51ba6)

---

## 🛠️ Features

### ✅ User Management & Authentication
- Secure registration, login, and logout
- Stateless authentication using JWT (JSON Web Tokens)
- Full data isolation across users

### 💸 Transaction Management
- Add, view, update, delete financial transactions
- Filter by date, category, and type (INCOME/EXPENSE)

### 🗂️ Category Management
- Built-in default categories (e.g., Salary, Food, Rent)
- Add/delete custom categories

### 🎯 Savings Goals
- Create and track savings goals
- Auto-progress tracking from income/expenses
- View completion % and remaining amount

### 📊 Reports & Analytics
- Monthly and yearly breakdown of incomes/expenses
- Net savings and category-wise reports

---

## 📦 Tech Stack

| Layer             | Technology                   |
|------------------|------------------------------|
| Language          | Java 17                      |
| Framework         | Spring Boot 3.x              |
| Security          | Spring Security              |
| Build Tool        | Maven                        |
| Database          | H2 (in-memory)               |
| Containerization  | Docker                       |
| Deployment        | Render                       |

---

## 🧱 Architecture

- Layered: `Controller → Service → Repository`
- DTO-based request/response mapping
- Centralized error handling with `@ControllerAdvice`
- Input validations with clear HTTP responses

---

## 🐳 Docker Support

### Build Docker Image
```bash
docker build -t personal-finance-manager .
```

### Push to Docker Hub (optional)
```bash
docker tag personal-finance-manager your-dockerhub-username/personal-finance-manager
docker push your-dockerhub-username/personal-finance-manager
```

---

## 🌍 Deployment on Render

- Dockerized image deployed on [Render](https://personal-finance-manager-9ja1.onrender.com)
- Persistent deployment with public API access
- Use API endpoints with the base URL: `https://your-live-url-here.com/api`

---

## 📘 API Overview

### 🔐 Auth Endpoints
- `POST /api/auth/register`
- `POST /api/auth/login`
- `POST /api/auth/logout`

### 💵 Transactions
- `GET /api/transactions`
- `POST /api/transactions`
- `PUT /api/transactions/{id}`
- `DELETE /api/transactions/{id}`

### 📁 Categories
- `GET /api/categories`
- `POST /api/categories`
- `DELETE /api/categories/{name}`

### 🎯 Goals
- `GET /api/goals`
- `POST /api/goals`
- `PUT /api/goals/{id}`
- `DELETE /api/goals/{id}`

### 📈 Reports
- `GET /api/reports/monthly/{year}/{month}`
- `GET /api/reports/yearly/{year}`

---

## 🧪 Run Tests

You can run all unit and integration tests using Maven. Ensure dependencies are installed and the project is built before executing tests.

### 🧼 Clean & Build Project

```bash
mvn clean install
```

### ▶️ Run All Tests

```bash
mvn test
```



## 📂 Project Structure

```
src/
 └── main/
     ├── java/
     │    └── com.yourdomain.finance/
     │          ├── controller/
     │          ├── service/
     │          ├── repository/
     │          ├── model/
     │          ├── dto/
     │          └── config/
     └── resources/
         └── application.properties
```

---

## 🤝 Contributing

Contributions are welcome! Please fork the repo and open a pull request.

---

## 🙋‍♂️ Author

**Aman Kumar**  
📧 [amanyadav880495@gmail.com](mailto:amanyadav880495@gmail.com)  
🔗 [GitHub Profile](https://github.com/SKYTOX07)

---
