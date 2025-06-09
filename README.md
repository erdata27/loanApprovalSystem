# Loan Approval System

A full-stack loan approval platform with user and admin panels, built using Spring Boot (Java) backend and React frontend. It features JWT-based authentication, rule-based and AI-based eligibility checks, and document management.

---

## 🚀 Tech Stack

### Backend
- Spring Boot
- Spring AI (for AI/ML-based eligibility scoring)
- Spring Security (JWT authentication & role-based access)
- Spring Data JPA (Hibernate)
- MySQL database

### Frontend
- React
- Axios
- Tailwind CSS / Bootstrap

### Tools
- Postman (API testing)
- Swagger (API documentation)
- IntelliJ IDEA (IDE)
- MySQL Workbench (Database design)
- GitHub (Version control)

---

## 📁 Project Structure (Backend)

```

loan-approval-system/
├── controller/
│   ├── AuthController.java
│   ├── LoanApplicationController.java
│   └── AdminController.java
├── model/
│   ├── User.java
│   ├── Role.java
│   ├── LoanApplication.java
│   └── Document.java
├── repository/
│   ├── UserRepository.java
│   ├── LoanApplicationRepository.java
│   └── DocumentRepository.java
├── service/
│   ├── AuthService.java
│   ├── LoanService.java
│   └── AdminService.java
├── config/
│   ├── SecurityConfig.java
│   └── JwtUtils.java
└── LoanApprovalSystemApplication.java

````

---

## ⚙️ Setup and Installation

### Prerequisites
- Java 17 (or 11)
- MySQL Server installed and running
- Node.js and npm (for frontend)
- Git

### Backend Setup

1. Clone the repo:

   git clone https://github.com/yourusername/loan-approval-system.git
   cd loan-approval-system


2. Create MySQL database:


   CREATE DATABASE loan_db;


3. Configure database in `src/main/resources/application.properties`:

   properties file
   
   spring.datasource.url=jdbc:mysql://localhost:3306/loan_db?useSSL=false&allowPublicKeyRetrieval=true&serverTimezone=UTC
   spring.datasource.username=your_mysql_username
   spring.datasource.password=your_mysql_password

   spring.jpa.hibernate.ddl-auto=update
   spring.jpa.show-sql=true

   jwt.secret=your_jwt_secret_key
   jwt.expirationMs=86400000
  

5. Build and run backend:

   bash
   ./mvnw spring-boot:run
   # or if using Gradle
   ./gradlew bootRun
   

6. Access Swagger UI to test APIs:

   
   
   

---

### Frontend Setup

1. Navigate to frontend folder (if separate):

   bash
   cd frontend
   

2. Install dependencies:

   bash
   npm install
   

3. Run the React app:

   bash
   npm start
   

4. Open your browser at http://localhost:3000

---

## 🔐 Authentication

* Uses JWT tokens.
* Role-based access control (USER, ADMIN).
* Secure endpoints with Spring Security.

---

## 🧪 Testing

* Backend tests with JUnit and Mockito.
* Test user registration, login, loan application, admin approval, eligibility rules.

---

## 📄 Features

* User Registration & Login
* Apply for loans with details & document upload
* View application status
* Admin dashboard to approve/reject loans
* Rule-based and AI-based loan eligibility scoring
* Secure REST APIs with JWT

---

## 📞 Contact

For any questions, reach out to erdata2005@outlook.com

---
