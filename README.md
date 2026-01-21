# Online Store Project

This is a Spring Boot web application for an Online Store.
It allows users to browse products, add them to a cart, check out, and manage products (Admin).

## Features
- User Authentication (Admin/User)
- Product CRUD with Image Uploads
- Shopping Cart & Checkout
- Email Notifications
- Spring Boot Application

A full-featured e-commerce platform built with **Spring Boot**, featuring user authentication, product management, shopping cart functionality, and order processing.

## Features

✅ **User Management**
- User registration with email and password
- Secure login with Spring Security
- Role-based access control (Admin & User roles)
- Password encryption using BCrypt

✅ **Product Management**
- Add/Edit/Delete products (Admin only)
- Product image upload with storage
- Product search and pagination
- Stock quantity tracking

✅ **Shopping Cart**
- Session-based shopping cart
- Add/Remove products from cart
- Quantity management
- Checkout functionality

✅ **Orders & Checkout**
- Order creation from cart
- Order history tracking
- Email notifications on checkout (optional)
- Order status management

✅ **Technical Features**
- RESTful API design
- Thymeleaf template engine
- Spring Data JPA with Hibernate
- H2 in-memory database (development)
- Bootstrap 4 responsive UI
- Custom error page handling
- HTTP method overrides for PUT/DELETE

---

## Technology Stack

| Technology | Version |
|-----------|---------|
| Spring Boot | 4.0.0 |
| Java | 17+ |
| Spring Security | Latest |
| Spring Data JPA | Latest |
| Hibernate | 7.1.8 |
| Thymeleaf | Latest |
| H2 Database | Latest |
| Maven | 3.9+ |

---

## Project Structure

```
src/main/java/com/store/
├── entity/              # JPA entities (User, Product, Order, OrderItem)
├── repository/          # Spring Data repositories
├── service/             # Business logic services
├── controller/          # HTTP controllers
├── config/              # Configuration classes
└── OnlineStoreApplication.java  # Main application class

src/main/resources/
├── templates/           # Thymeleaf HTML templates
└── application.properties  # Configuration file
```

---

## Setup Instructions

### Prerequisites

- **Java 17+** installed
- **Maven 3.9+** installed

### 1. Build the Project

```bash
cd "/Users/janiduperera/Downloads/demo 4"
mvn -DskipTests clean package
```

### 2. Run the Application

```bash
java -jar target/demo-0.0.1-SNAPSHOT.jar
```

The application will start on **http://localhost:8080**

### 3. Default Admin Credentials

Upon startup, the application creates a default admin user:

- **Email:** `admin@store.com`
- **Password:** `password123`

---

## Usage Guide

### Home Page
- View all available products
- Search products by name
- Admin can add/delete products

### User Registration
1. Click **Register** 
2. Enter email and password
3. Submit to create account

### Admin Login
1. Click **Login**
2. Enter admin credentials
3. Click "Add New Product" to manage inventory

### Add Product
1. Fill product details
2. Upload product image
3. Click **Save**

### Shopping Cart
- Add products to cart
- View cart contents
- Proceed to checkout

### Logout
Click **Logout** to exit session.

---

## API Documentation

A Postman collection is available at `docs/postman_collection.json`.

**Key Endpoints:**

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/` | Home page |
| GET | `/login` | Login page |
| POST | `/login` | Submit login |
| GET | `/register` | Registration page |
| POST | `/saveUser` | Create user |
| GET | `/showNewProductForm` | Add product form |
| POST | `/saveProduct` | Save product |
| DELETE | `/deleteProduct/{id}` | Delete product |
| GET | `/cart` | View cart |
| POST | `/addToCart` | Add to cart |
| POST | `/logout` | Logout |

---

## Database

The application uses an **H2 in-memory database** for development.

**Tables:**
- `user` - User accounts and roles
- `product` - Product catalog
- `order` - Customer orders
- `order_item` - Order items

---

## Security Configuration

- **Form-based login** with email
- **BCrypt password encoding**
- **Role-based access control** (ADMIN, USER)
- **CSRF protection** enabled
- **Session-based authentication**

---

## Troubleshooting

### Login issues
- Use email field as username
- Default credentials: `admin@store.com` / `password123`

### Image upload fails
- Check file size limits in `application.properties`
- Ensure `product-images/` folder exists

### Logout error
- Ensure logout form uses POST method
- Clear browser cookies if needed

---

## Git Commit History

```bash
git log --oneline
# Initial project setup with Maven and Spring Boot configuration
```

---

## Submission Checklist

- ✅ Custom `error.html` created
- ✅ HTTP method overrides enabled
- ✅ Postman collection exported
- ✅ README.md with setup instructions
- ✅ Git repository initialized
- ✅ Clean package structure
- ✅ Application runs successfully

---

**Created:** December 2025  
**Version:** 1.0.0

## Project Abstract

This project is a full-stack E-Commerce Web Application developed using the Spring Boot framework. Designed to simulate a real-world online retail environment, the application features a robust Role-Based Access Control (RBAC) system, distinguishing between Administrator and Customer workflows using Spring Security. Core functionalities include comprehensive product management (CRUD), a session-based shopping cart, and secure user authentication. To exceed standard requirements, the system integrates advanced features such as dynamic file uploads for product imagery and automated email notifications upon order completion. The application follows a layered architecture (Controller-Service-Repository) and enforces data integrity through Bean Validation and strictly typed JPA entities. Reliability is ensured through a suite of automated integration tests validating security, validation logic, and file handling.


Submission: added abstract and minor formatting
