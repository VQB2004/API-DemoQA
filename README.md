# 📘 DemoQA Bookstore API Test

## 🧩 Overview
This project automates API testing for the **DemoQA Book Store API** using **Postman**, **Newman**, and **GitHub Actions** for CI/CD integration. 

---

## 🚀 Test Scope

### 🔹 Main Endpoints
| Module | Endpoint | Description |
|--------|-----------|-------------|
| **User** | `/Account/v1/User` | Create, Get, and Delete users |
| **Token** | `/Account/v1/GenerateToken` | Generate authentication token |
| **Book** | `/BookStore/v1/Books`, `/BookStore/v1/Book` | Retrieve, Add, Update, and Delete books |

### 🔹 Main Scenarios
1. User Management  
2. Authentication  
3. Book Management  
4. Book Collection  
5. End-to-End Flow  
6. Error Handling  

---

## 🧪 Test Approach
| Category | Details |
|-----------|----------|
| **Method** | Black-box testing |
| **Type** | Functional & Negative |
| **Toolset** | Postman v11, Newman CLI, GitHub Actions |
| **Reporting** | CLI output + HTML report (via newman-reporter-htmlextra) |
| **Execution** | Automated on each push/pull request via CI/CD |

---

## ⚙️ Environment
| Component | Description |
|------------|-------------|
| **Base URL** | [https://demoqa.com/swagger](https://demoqa.com/swagger) |
| **Authorization** | Bearer Token |
| **OS** | Windows 11 |
| **Browser** | Chrome 141 |

---

## 🧰 CI/CD Workflow
Automated tests are triggered by **GitHub Actions** on every push or pull request to the `main` branch.  
Each run:
1. Installs Newman & reporter  
2. Executes all Postman test folders  
3. Generates HTML reports in `/reports`
