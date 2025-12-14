#  Kata Sweet Shop Management System

A **full-stack web application** designed to manage a sweet shop efficiently. The system supports secure customer authentication, a dynamic product catalog, inventory management, and a smooth purchase workflow. It is built using **Django REST Framework** for the backend and **React** for the frontend.

This project demonstrates real-world full-stack development practices, RESTful API design, JWT-based authentication, and responsive UI development.

---

## 📌 Table of Contents

* Overview
* Features
* Tech Stack
* Project Architecture
* Screenshots
* Installation & Setup
* API Endpoints
* Testing Strategy
* AI-Assisted Development
* Challenges & Learnings
* Common Issues
* Future Enhancements
* License

---

## 📖 Overview

The **Kata Sweet Shop Management System** is a web-based application that allows customers to browse and purchase sweets online while enabling administrators to manage products and inventory. The application follows a **client–server architecture**, ensuring scalability, maintainability, and security.

---

## ✨ Features

### 🛍️ Customer Features

* Secure **User Registration & Login** using JWT authentication
* Browse sweets with images, prices, categories, and availability
* Advanced **Search & Filtering** (by name, category, price, stock)
* Purchase sweets in **kg/grams** with real-time stock updates
* View personal **purchase history**
* Fully **responsive UI** built with Bootstrap

### 🔧 Admin Features

* Add, update, and delete sweet products
* Upload and manage product images
* Monitor inventory levels and sales
* Prevent purchases when items are out of stock

---

## 🛠️ Tech Stack

### Backend

* **Django 5.1.7** – Web framework
* **Django REST Framework (DRF)** – REST API development
* **SQLite** – Database
* **JWT Authentication** – Secure user authentication
* **Pillow** – Image handling
* **django-cors-headers** – CORS support

### Frontend

* **React 18** – User interface
* **React Router DOM** – Client-side routing
* **Axios** – API communication
* **Bootstrap 5** – Responsive UI styling
* **Local Storage** – Token persistence

---

## 🏗️ Project Architecture

```
AI-Kata-Sweet-Shop/
├── sweetshop_backend/
│   ├── api/                     # Models, serializers, views
│   ├── sweetshop_backend/       # Project settings
│   ├── media/                   # Uploaded images
│   ├── manage.py
│   └── requirements.txt
│
└── sweetshop_frontend/
    ├── src/
    │   ├── components/          # React components
    │   ├── context/             # Authentication context
    │   ├── utils/               # API helpers
    │   └── App.js
    └── package.json
```

---

## 📸 Screenshots

### Welcome Page

<img src="https://github.com/user-attachments/assets/80a1bd2e-7dd0-4e47-bf5b-3b2a047e8c23" />

### Register Page

<img src="https://github.com/user-attachments/assets/983e1941-c16b-462a-beae-341b46b04187" />

### Login Page

<img src="https://github.com/user-attachments/assets/d5994854-9def-412d-bc6d-e380405bbe1a" />

### Customer Dashboard

<img src="https://github.com/user-attachments/assets/f4e2a10f-d407-4d86-b9eb-4540a4f695c5" />

### Purchase Flow

<img src="https://github.com/user-attachments/assets/c909ee65-3152-4cb8-918d-6e8428ef3427" />

### Out of Stock Handling

<img src="https://github.com/user-attachments/assets/f27aa844-eed3-4572-91b9-91310f4232c6" />

### Admin Interface

<img src="https://github.com/user-attachments/assets/9198fa8f-05e3-412a-bc35-6be704760e54" />

---

## 🚀 Installation & Setup

### Prerequisites

* Python 3.10+
* Node.js 18+
* npm or yarn

### Backend Setup

```bash
cd sweetshop_backend
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py create_sample_data
python manage.py runserver
```

### Frontend Setup

```bash
cd sweetshop_frontend
npm install
npm start
```

The backend will run at `http://127.0.0.1:8000` and the frontend at `http://localhost:3000`.

---

## 🔌 API Endpoints

| Method | Endpoint                     | Description           |
| ------ | ---------------------------- | --------------------- |
| POST   | `/api/register/`             | User registration     |
| POST   | `/api/login/`                | User login            |
| GET    | `/api/sweets/simple/`        | Fetch all sweets      |
| POST   | `/api/sweets/<id>/purchase/` | Purchase a sweet      |
| GET    | `/api/purchases/user/`       | User purchase history |

---

## 🧪 Testing Strategy (TDD)

* **Unit Tests**: Models and utility functions
* **Integration Tests**: API endpoints and authentication
* **Frontend Tests**: React components using Jest

### Test Coverage

* Backend APIs: ~85%
* Frontend components: ~70%
* Database operations: ~90%

---

## 🤖 AI-Assisted Development

### Tools Used

* **Claude Sonnet 4** – Primary AI assistant
* **GitHub Copilot** – Code suggestions
* **ChatGPT** – Debugging and documentation support

### Role of AI

* Generated Django models, serializers, and views
* Assisted in React component creation
* Helped debug JWT authentication and CORS issues
* Supported documentation and README creation

---

## 📚 Challenges & Learnings

### Challenges

* JWT authentication setup
* CORS configuration between frontend and backend
* Decimal and float handling in purchase logic
* Structuring reusable React components

### Learnings

* Importance of API security
* Value of Test-Driven Development
* Best practices for full-stack architecture
* Effective use of AI as a development assistant

---

## 🔧 Common Issues

1. **Authentication Errors** – Verify JWT and token headers
2. **CORS Issues** – Ensure correct `django-cors-headers` settings
3. **Migration Errors** – Run migrations after model changes
4. **Image Upload Problems** – Check Pillow installation and media paths

---

## 🚧 Future Enhancements

* Payment gateway integration
* Role-based access control
* Order invoice generation
* Deployment using Docker and cloud services

---

## 📜 License

This project is licensed under the **MIT License**. You are free to use, modify, and distribute this project for educational use.
