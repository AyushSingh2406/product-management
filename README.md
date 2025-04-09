# 📦 Product Management System

A full-stack Product Management application that allows users to perform CRUD operations (Create, Read, Update, Delete) on products with authentication and a clean, responsive UI. Built using the **MERN Stack** (MongoDB, Express, React, Node.js).

---

## 🚀 Features

- ✅ User Authentication (JWT-based)
- 🛒 Add / View / Update / Delete Products
- 🔐 Protected Routes for Authenticated Users
- 📱 Responsive Design
- 💾 Persistent Data (MongoDB Atlas or Local)
- 📊 Product Listing in Table/Grid
- 🎨 Clean and Interactive UI

---

## 🛠 Tech Stack Used

| **Frontend**          | **Backend**        | **Database**      | **Other Tools**    |
|-----------------------|--------------------|-------------------|--------------------|
| React.js (Hooks)      | Node.js            | MongoDB (Atlas)   | Git & GitHub       |
| React Router DOM      | Express.js         | Mongoose          | Postman (Testing)  |
| Axios                 | JWT Authentication |                   | VS Code (Editor)   |
| Bootstrap / CSS       | bcrypt.js          |                   | dotenv (Env Vars)  |

---

## 🧑‍💻 Folder Structure

```
Product_Management/
├── client/               # Frontend (React)
│   ├── src/
│   │   ├── components/   # React components for UI
│   │   ├── pages/        # Pages (Login, Dashboard, etc.)
│   │   ├── App.js        # Main app component
│   │   └── index.js      # Entry point of React app
├── server/               # Backend (Node/Express)
│   ├── controllers/      # Logic for API requests
│   ├── models/           # Mongoose schemas for MongoDB
│   ├── routes/           # Express routes
│   ├── server.js         # Main server file
│   └── .env              # Environment variables
├── README.md             # Project overview
└── package.json          # NPM dependencies and scripts
```

---

## ⚙️ How to Run Locally

### 🖥️ Prerequisites

- Node.js (v14 or higher)
- MongoDB (local instance or MongoDB Atlas)
- Git
- Postman (for API testing)

---

### 🔧 Backend Setup (Node.js + Express + MongoDB)

1. **Clone the repository:**
   ```bash
   git clone https://github.com/AyushSingh2406/product-management.git
   cd product-management
   ```

2. **Navigate to the `server` directory:**
   ```bash
   cd server
   ```

3. **Install backend dependencies:**
   ```bash
   npm install
   ```

4. **Create a `.env` file** in the `server/` directory with the following content:
   ```env
   MONGO_URI=your_mongo_connection_string
   JWT_SECRET=your_jwt_secret_key
   PORT=5000
   ```

   - Replace `your_mongo_connection_string` with your MongoDB Atlas connection string or local MongoDB URI.
   - Replace `your_jwt_secret_key` with a secret string for JWT authentication.

5. **Start the backend server:**
   ```bash
   npm start
   ```

   The backend will run on `http://localhost:5000`.

---

### 🎨 Frontend Setup (React)

1. **Navigate to the `client` directory:**
   ```bash
   cd client
   ```

2. **Install frontend dependencies:**
   ```bash
   npm install
   ```

3. **Start the frontend server:**
   ```bash
   npm start
   ```

   The React app will run on `http://localhost:3000`.

---

## 🔐 Environment Variables (`.env`)

### Backend (`server/.env`)

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
PORT=5000
```

### Frontend (`client/src/config.js`)

If you want to store the backend API URL in the frontend configuration:

```js
const API_URL = "http://localhost:5000";
```

---

## 📦 API Endpoints

| **Method** | **Route**               | **Description**                        | **Access**       |
|------------|-------------------------|----------------------------------------|------------------|
| POST       | `/api/auth/register`     | Register a new user                   | Public           |
| POST       | `/api/auth/login`        | Login with credentials                | Public           |
| GET        | `/api/products`          | Get all products                       | Private (JWT)    |
| POST       | `/api/products`          | Create a new product                   | Private (JWT)    |
| PUT        | `/api/products/:id`      | Update product by ID                  | Private (JWT)    |
| DELETE     | `/api/products/:id`      | Delete product by ID                  | Private (JWT)    |

---


## 🧠 Future Enhancements

- ✅ Search & Filter Products
- 📤 Image Upload for Products
- 📈 Admin Dashboard with Charts
- 🌍 Multi-language Support
- 🛠 Unit & Integration Tests

---

## 🤝 Contributing

We welcome contributions from the community! If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-name`).
3. Make your changes.
4. Commit your changes (`git commit -m 'Add new feature'`).
5. Push to the branch (`git push origin feature-name`).
6. Open a Pull Request.

---

## 📄 License

This project is licensed under the MIT License.

---

## 🙋‍♂️ Author

- **GitHub:** [AyushSingh2406](https://github.com/AyushSingh2406)
- **Email:** ayushsingh2004.abs@gmail.com

---
