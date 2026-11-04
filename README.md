# Django E-Commerce Website

A full-stack E-Commerce web application built using Django REST Framework and React. The application allows users to browse products, explore categories, manage shopping carts, authenticate securely, and place orders.

## 🚀 Features

- User Registration and Login
- JWT Authentication
- Product Listing
- Product Details
- Product Categories
- Shopping Cart Management
- Add, Update, and Remove Cart Items
- Checkout and Order Creation
- Protected Routes
- RESTful API Integration

## 🛠️ Technologies Used

### Frontend
- React.js
- React Router
- Vite
- Tailwind CSS
- JavaScript

### Backend
- Python
- Django
- Django REST Framework
- Django REST Framework Simple JWT

### Database
- PostgreSQL

### Other Tools
- Git and GitHub
- VS Code
- Postman

## 📁 Project Structure

```text
django-ecommerce-project/
│
├── backend/
│   ├── backend/
│   │   ├── settings.py
│   │   ├── urls.py
│   │   └── ...
│   │
│   ├── store/
│   ├── manage.py
│   └── requirements.txt
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   └── utils/
│   │
│   └── package.json
│
└── .gitignore
```

## ⚙️ Installation and Setup

### 1. Clone the Repository

```bash
git clone https://github.com/Mihir3302/django-ecommerce-project.git
```

Navigate into the project:

```bash
cd django-ecommerce-project
```

### 2. Backend Setup

Open a terminal and navigate to the backend:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the virtual environment on Windows:

```bash
venv\Scripts\activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

### 3. Configure Environment Variables

Create a `.env` file inside the `backend` directory.

Add your local configuration:

```env
DJANGO_SECRET_KEY=your_django_secret_key
DB_NAME=your_database_name
DB_USER=your_database_username
DB_PASSWORD=your_database_password
DB_HOST=localhost
DB_PORT=5432
```

Replace the values with your own local PostgreSQL and Django configuration.

### 4. Database Migration

Run:

```bash
python manage.py makemigrations
python manage.py migrate
```

### 5. Start the Django Server

```bash
python manage.py runserver
```

Backend server:

```text
http://127.0.0.1:8000/
```

### 6. Frontend Setup

Open another terminal and navigate to the frontend:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the frontend development server:

```bash
npm run dev
```

Open the local URL displayed by Vite in your terminal (usually `http://localhost:5173/`).

## 🔑 Demo Login Credentials

| Field | Value |
|---|---|
| Username | Rahul |
| Password | Rahul@23 |

**Note:** These are intended as demo credentials. The account must exist in your local database. If it does not, register the user through the signup page first. Do not use these credentials for production.

## 🔗 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/register/` | User registration |
| POST | `/api/token/` | User login |
| POST | `/api/token/refresh/` | Refresh JWT token |
| GET | `/api/products/` | Get all products |
| GET | `/api/products/<id>/` | Get product details |
| GET | `/api/categories/` | Get all categories |
| GET | `/api/cart/` | Get shopping cart |
| POST | `/api/cart/add/` | Add item to cart |
| POST | `/api/cart/remove/` | Remove cart item |
| POST | `/api/cart/update/` | Update cart item |
| POST | `/api/orders/create/` | Create an order |

## 🛒 Order and Payment

The application supports order creation with Cash on Delivery (COD) and an Online payment option in the checkout flow.

**Note:** An external payment gateway integration is not included.

## 🔒 Security

- JWT-based authentication
- Protected frontend routes
- Environment variables for sensitive configuration
- `.env` files excluded from Git tracking using `.gitignore`

Never commit your actual `.env` files, database passwords, or Django secret keys to GitHub.

## 👨‍💻 Author

**Mihir Ramani**

GitHub: [Mihir3302](https://github.com/Mihir3302)

Project Repository: [Django E-Commerce Project](https://github.com/Mihir3302/django-ecommerce-project)

---

⭐ If you find this project useful, consider giving the repository a star!