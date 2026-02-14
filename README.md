# 🛒 Premium Online Store Project - Team Edition

A professional, high-end E-commerce application built with **Spring Boot**, **Thymeleaf**, and **Modern CSS**. This repository is organized for a collaborative team of 10 developers, each with their own dedicated workspace.

## 📁 Project Structure & Assignments

The project is split into 10 independent modules. Each member is responsible for their respective folder:

### **Phase 1: Infrastructure & Auth**
*   **Member 01: Setup & Infrastructure** (`Member_01_Setup_Infra`)
    *   Project architecture, lead configuration, and documentation.
*   **Member 02: Backend Security** (`Member_02_Security_Back-end`)
    *   Spring Security, Authentication, and User Authorization logic.
*   **Member 03: User Management UI** (`Member_03_Auth_Frontend`)
    *   Premium Login and registration page design.

### **Phase 2: Product & Catalog**
*   **Member 04: Product Backend** (`Member_04_Product_Back-end`)
    *   Product Entity, Repositories, and Catalog Service.
*   **Member 05: Product Frontend** (`Member_05_Product_Frontend`)
    *   Dynamic Shop Grid and Product Details UI.

### **Phase 3: Commerce & Search**
*   **Member 06: Shopping Cart** (`Member_06_Shopping_Cart`)
    *   Cart logic and Session management.
*   **Member 07: Orders & Checkout** (`Member_07_Orders_Check-out`)
    *   Transaction flow and order history.
*   **Member 08: Search & Uploads** (`Member_08_Search_Uploads`)
    *   "Beyond CRUD": Advanced filtering and Image upload system.

### **Phase 4: Stability & Analytics**
*   **Member 09: QA & Validation** (`Member_09_Validation_QA`)
    *   Global error handling (404/500/403) and unit testing.
*   **Member 10: Reporting & Notifications** (`Member_10_Reporting_Notifications`)
    *   "Beyond CRUD": Sales analytics and Email/SMS notifications.

---

## 🛠 Technical Requirements

- **Backend**: Spring Boot (Layered Architecture: Controller → Service → Repository → Entity).
- **Security**: Spring Security for Auth & Auth (cookie/session).
- **Validation**: Robust server-side and client-side validation for all forms.
- **Reliability**: Graceful handling of 404, 400, and 401/403 errors using `@ControllerAdvice`.

## 🚀 How to Run (For Members)

1.  **Navigate** to your specific `Member_XX` folder.
2.  **Run** the application:
    ```bash
    ./mvnw spring-boot:run
    ```
3.  **Access** the store at `http://localhost:8080`.

---

## 📦 Submission Package Requirements
As per the assignment rules, each member must ensure their folder contains:
1.  **Full Source Code** with clear package naming and no dead code.
2.  **README.md** with setup steps, run instructions, and screenshots.
3.  **Postman Collection** (if applicable) for API testing.
