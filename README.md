# Blog Server 🚀

**Live Link**: [https://a3-blog-server.vercel.app/](https://a3-blog-server.vercel.app/)

A backend for a blog application that supports user authentication, blog management, and user blocking functionality. This project is built with **Node.js**, **Express**, **MongoDB** (via Mongoose), and **TypeScript**.

---

## ✨ Features

- **User Authentication**:  
  Users can register, log in, and manage their sessions.
- **Role-Based Access Control**:  
  Users have different roles (`admin`, `user`) with varying access levels.
- **Blog Management**:  
  Admins and users can create, update, delete, and view blogs.
- **User Management**:  
  Admins can block users.

---

## 🛠️ Requirements

- **Node.js** (>=16.x)
- **MongoDB** instance (local or cloud)

---

## 🚀 Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/parvejme24/a3-blog-server.git
   ```

2. Navigate to the project directory:

   ```bash
   cd a3-blog-server
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Create a `.env` file in the root directory and add the following environment variables:

   ```env
   DATABASE_URL=your_mongodb_connection_string
   NODE_ENV=development
   PORT=5050
   JWT_ACCESS_SECRET=your_jwt_secret
   JWT_ACCESS_EXPIRES_IN=time
   ```

5. Start the development server:

   ```bash
   npm run dev
   ```

---

## 📚 Available Scripts

- **`npm run dev`**: Start the server in development mode.
- **`npm run build`**: Build the project for production.
- **`npm start`**: Start the server in production mode.

---

## 🔐 Environment Variables

| Variable                | Description                   |
| ----------------------- | ----------------------------- |
| `PORT`                  | Port on which the server runs |
| `DATABASE_URL`          | MongoDB connection string     |
| `JWT_ACCESS_SECRET`     | Secret key for JWT token      |
| `JWT_ACCESS_EXPIRES_IN` | JWT expiration time           |

---

## 🏗️ Project Structure

```bash
├── src
│   ├── controllers
│   ├── models
│   ├── routes
│   ├── middlewares
│   ├── utils
│   └── index.ts
├── .env
├── .gitignore
├── package.json
└── tsconfig.json
```

---

## 📄 API Endpoints

### Auth Routes

| Method | Endpoint           | Description         |
| ------ | ------------------ | ------------------- |
| POST   | /api/auth/register | Register a new user |
| POST   | /api/auth/login    | Login a user        |

### Blog Routes

| Method | Endpoint       | Description             |
| ------ | -------------- | ----------------------- |
| GET    | /api/blogs     | Get all blogs           |
| POST   | /api/blogs     | Create a new blog       |
| PUT    | /api/blogs/:id | Update an existing blog |
| DELETE | /api/blogs/:id | Delete a blog           |

### User Routes

| Method | Endpoint             | Description   |
| ------ | -------------------- | ------------- |
| GET    | /api/users           | Get all users |
| PATCH  | /api/users/:id/block | Block a user  |

---

## 🤝 Contributions

Contributions are welcome! Please fork the repository and submit a pull request.

---

## 📄 License

This project is licensed under the **MIT License**.

---

## 💬 Contact

If you have any questions, feel free to reach out:

- **GitHub**: [parvejme24](https://github.com/parvejme24)
- **Email**: parvej@example.com
