Got it! Here's an improved **README.md** with a clear, detailed **Project Structure** section included:


# 🚀 Loan Approval System

A full-stack **Loan Approval System** built with **Spring Boot**, **MongoDB**, and **React** — designed for managing loan applications with secure authentication, admin controls, and optional AI-based eligibility scoring.

---

## 🛠️ Tech Stack

| Backend                                   | Frontend                 | Tools & Utilities                  |
|-------------------------------------------|--------------------------|----------------------------------|
| ![Java](https://img.shields.io/badge/Java-ED8B00?logo=java&logoColor=white) JAVA |![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?logo=spring&logoColor=white) SpringBoot|![React](https://img.shields.io/badge/React-20232A?logo=react&logoColor=61DAFB) React.js | ![Postman](https://img.shields.io/badge/Postman-FF6C37?logo=postman&logoColor=white) Postman | ![MongoDB](https://img.shields.io/badge/MongoDB-47A248?logo=mongodb&logoColor=white) MongoDB    | 
![Axios](https://img.shields.io/badge/Axios-5A29E4?logo=axios&logoColor=white) Axios | ![Swagger](https://img.shields.io/badge/Swagger-85EA2D?logo=swagger&logoColor=black) Swagger UI|
| ![Spring Security](https://img.shields.io/badge/Spring_Security-6DB33F?logo=springsecurity&logoColor=white) Spring Security | ![Tailwind](https://img.shields.io/badge/Tailwind_CSS-38B2AC?logo=tailwind-css&logoColor=white) Tailwind CSS  | ![GitHub](https://img.shields.io/badge/GitHub-181717?logo=github&logoColor=white) GitHub                 |
| ![Spring AI (Experimental)](https://img.shields.io/badge/Spring_AI-6DB33F?logo=spring&logoColor=white) Spring AI  |

---

## 🌟 Features

### User Panel
- 🔐 Secure **Register/Login** with JWT-based authentication
- 💰 Apply for loans: enter amount, term, income, employment status, upload documents
- 📄 View application status & track uploaded documents

### Admin Panel
- 📊 Dashboard with loan application list & filters
- 👤 View user details & loan applications
- ✔️ Manual or **rule-based eligibility checks**
- ✅ Approve/Reject loans with remarks
- 📥 Download uploaded documents
- 🤖  AI-based eligibility scoring using Spring AI 

---

## 📁 Project Structure

```plaintext
loan-approval-system/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── loanApprovalSystem/
│   │   │           ├── LoanApprovalSystemApplication.java
│   │   │           ├── config/
│   │   │           │   ├── SecurityConfig.java                  # Spring Security config
│   │   │           │   ├── OpenAIConfig.java                    # OpenAI API configuration
│   │   │           ├── controller/
│   │   │           │   ├── AuthController.java
│   │   │           │   ├── LoanApplicationController.java
│   │   │           │   ├── AdminController.java
│   │   │           ├── dto/
│   │   │           │   ├── LoanApplicationRequest.java          # DTO for loan application input
│   │   │           │   ├── EligibilityResponse.java             # DTO for AI eligibility result
│   │   │           ├── exception/
│   │   │           │   ├── BadRequestException.java
│   │   │           │   ├── ResourceNotFoundException.java
│   │   │           │   ├── GlobalExceptionHandler.java
│   │   │           ├── model/
│   │   │           │   ├── User.java
│   │   │           │   ├── Role.java
│   │   │           │   ├── LoanApplication.java
│   │   │           │   ├── Document.java
│   │   │           ├── repository/
│   │   │           │   ├── UserRepository.java
│   │   │           │   ├── LoanApplicationRepository.java
│   │   │           │   ├── DocumentRepository.java
│   │   │           ├── security/
│   │   │           │   ├── JwtUtils.java
│   │   │           │   ├── JwtAuthenticationFilter.java
│   │   │           │   ├── CustomUserDetailsService.java
│   │   │           ├── service/
│   │   │           │   ├── AuthService.java
│   │   │           │   ├── LoanService.java
│   │   │           │   ├── AdminService.java
│   │   │           │   ├── EligibilityService.java              # Business logic including AI integration
│   │   │           ├── rules/
│   │   │           │   ├── EligibilityRule.java
│   │   │           │   ├── IncomeRule.java
│   │   │           │   ├── TermRule.java
│   │   │           │   ├── AmountRule.java
│   │   ├── resources/
│   │   │   ├── application.properties                           # Configuration file
│   │   │   ├── static/
│   │   │   ├── templates/
│   │   │   ├── logback-spring.xml                              # Logging config
│   ├── test/
│       ├── java/
│       │   └── com/
│       │       └── loanApprovalSystem/
│       │           ├── service/
│       │           │   ├── LoanServiceTests.java
│       │           │   ├── EligibilityServiceTests.java
│       │           ├── controller/
│       │               ├── LoanApplicationControllerTests.java
│       ├── resources/
├── .gitignore
├── build.gradle or pom.xml                                     # Build file (Gradle/Maven)
├── README.md


````

---

## ⚙️ Getting Started

### Prerequisites

* Java 17+
* MongoDB (locally or cloud)
* Node.js and npm (for frontend)
* Maven or Gradle

### Run Backend

```bash
# Clone repo
git clone https://github.com/yourusername/loan-approval-system.git
cd loan-approval-system/backend

# Configure MongoDB URI in application.properties
# Build and run
./mvnw spring-boot:run
```

### Run Frontend

```bash
cd ../frontend
npm install
npm start
```

---

## 🧪 Testing

* Use **Postman** for API testing (import provided collection)
* Run JUnit tests with Mockito for service and controller layer

---

## 📄 API Documentation

Swagger UI available at: ``

---

## 🚀 Optional Add-ons

* Email notifications via **JavaMailSender**
* Document storage with **AWS S3** or **Firebase Storage**
* PDF generation of loan application summary
* Logging and monitoring using **ELK Stack** or **Prometheus**

---

## 👨‍💻 Contributing

Contributions are welcome! Please fork the repo and create a pull request.

---


## 📞 Contact

Created by **ESWAR** - erdata2005@outlook.com

---

Made with ❤️ using Spring Boot & React!

