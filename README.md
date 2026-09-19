# 🧪 QA Automation Portfolio: PetStore API Testing & Automation

> About this repository: This project demonstrates automated API testing using Postman and JavaScript test scripts (Chai assertions) for the Swagger PetStore v3 service. It covers essential CRUD operations including fetching pet records by valid and invalid IDs, and adding new pets to the store inventory. It also highlights a modern "Shift-Left" QA approach and Continuous Integration (CI/CD) readiness via Newman.

![Postman](https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Newman](https://img.shields.io/badge/Newman-026E42?style=for-the-badge&logo=postman&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=github-actions&logoColor=white)

## 🎯 Project Overview

This collection provides automated API test scripts targeting the Swagger PetStore v3 API (`https://petstore3.swagger.io`). It validates core inventory management endpoints, data payloads, and response statuses.

As a QA Automation / API Testing Engineer, my focus in this repository is to implement clean automated assertions, test positive and negative scenarios, and ensure reliable REST API contract validation.

## 🛠️ QA Tech Stack & Tools

* **API Testing Tool:** Postman
* **CLI Runner / CI Execution:** Newman
* **Test Assertions & Scripting:** JavaScript (Chai Assertion Library built into Postman)
* **CI/CD Pipeline Support:** GitHub Actions
* **Target Environment:** Swagger PetStore v3 REST API

## 📊 Test Strategy & Coverage

### 1. Automated API Testing & Assertions
The Postman collection includes structured test suites (`pm.test`) validating:
* **Get Pet By Valid Id (`GET /api/v3/pet/78`):** Verifies successful retrieval of existing pet records, expecting an HTTP 200 OK status.
* **Get Pet By Invalid Id (`GET /api/v3/pet/100`):** Validates negative testing scenarios and error handling behavior, expecting an HTTP 500 status response for non-existent or invalid pet IDs.
* **Add New Pet (`POST /api/v3/pet`):** Tests resource creation by sending a JSON payload containing pet details (name: "Dogly", category, status: "available"), verifying successful creation with an HTTP 200 OK status.

## 🚀 How to Run the Tests Locally

To run and evaluate this Postman collection locally using Node.js and Newman, follow these steps:

### 1. Prerequisites
Ensure you have Node.js installed, then install Newman globally (if not already installed):
```bash
npm install -g newman
