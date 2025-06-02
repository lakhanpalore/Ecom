# 🛒 MERN Stack E-commerce Website

This is a complete **E-commerce web application** built using the MERN stack (MongoDB, Express, React, Node.js). It includes all essential features for online shopping: product listings, cart management, checkout, user authentication, and an admin dashboard for order and product management.

> 🚀 Project Status: In development  
> 🌐 Live Demo: _Coming Soon_

---

## 📌 Key Features

### 🧑 User Features
- User registration and login with JWT-based authentication
- Browse products by category or name
- View product details
- Add and remove products from cart
- Checkout with summary and simulated payment

### 🛠 Admin Features
- Admin login with secure routes
- Add, update, and delete products
- View all orders placed by users
- Manage users and inventory

---

## 🧰 Tech Stack

| Layer     | Technology            |
|-----------|------------------------|
| Frontend  | React, React Router, Bootstrap |
| Backend   | Node.js, Express.js    |
| Database  | MongoDB + Mongoose     |
| Authentication | JWT, bcryptjs     |
| State Management | Context API / Redux (optional) |
| Tools     | Nodemon, dotenv        |

---

## 📁 Project Structure

Ecom/
├── client-main/ # React frontend
│ ├── public/ # Public assets
│ └── src/ # React components and pages
│ ├── components/ # Reusable components
│ ├── pages/ # Home, Cart, Login, etc.
│ ├── App.js # Main App component
│ └── index.js # Entry point
│
├── server-master/ # Express backend
│ ├── controllers/ # Business logic
│ ├── models/ # Mongoose schemas
│ ├── routes/ # API routes (product, user, order)
│ ├── middleware/ # Auth, error handling
│ ├── config/ # DB connection
│ └── server.js # Entry point for backend


---

## 🔧 Setup Instructions

### 🖥️ Backend (Express + MongoDB)

1. Navigate to the backend folder:

```bash
cd server-master
npm install
```

2. Environment Variables
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret_key

```bash
cd ../client-main
npm run dev
```
🌐 Deployment
You can deploy this app using:

Frontend:
 Netlify

 Vercel

 Render (static build)

Backend:
 Render

 Railway

 Heroku

Database:
Use MongoDB Atlas (cloud-hosted MongoDB)

🛠 REST API Endpoints
🔐 Auth
Method	Endpoint	Description
POST	/api/auth/register	Register user
POST	/api/auth/login	Login user

🛍 Products
Method	Endpoint	Description
GET	/api/products	Get all products
GET	/api/products/:id	Get single product
POST	/api/products	Add new product (admin)
PUT	/api/products/:id	Update product (admin)
DELETE	/api/products/:id	Delete product (admin)

🧾 Orders
Method	Endpoint	Description
POST	/api/orders	Create new order
GET	/api/orders	Get all orders (admin)


