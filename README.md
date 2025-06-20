
# Student Management System API

A simple RESTful API built with **Node.js**, **Express**, and **MongoDB** (via **Mongoose**) to manage student records.

## 🚀 Features

- Create, read, update, and delete (CRUD) student records
- MongoDB integration with Mongoose
- CORS-enabled for cross-origin requests
- Environment configuration using dotenv

## 🛠 Tech Stack

- **Node.js**
- **Express**
- **MongoDB**
- **Mongoose**
- **body-parser**
- **cors**
- **dotenv**

## 📂 Project Structure

```
.
├── models
│   └── Student.js        # Mongoose schema for student
├── routes
│   └── students.js       # API routes for student operations
├── server.js             # Express server setup
├── package.json
└── package-lock.json
```

## 📦 Installation

1️⃣ Clone the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

2️⃣ Install dependencies:

```bash
npm install
```

3️⃣ Create a `.env` file in the root directory:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

## ▶️ Running the Server

```bash
node server.js
```

The server will start on `http://localhost:5000` (or the port you specify in `.env`).

## 📌 API Endpoints

| Method | Endpoint             | Description              |
|--------|----------------------|--------------------------|
| POST   | `/api/students`       | Create a new student     |
| GET    | `/api/students`       | Get all students         |
| PUT    | `/api/students/:id`   | Update student by ID     |
| DELETE | `/api/students/:id`   | Delete student by ID     |

## 💡 Example Request Body

For `POST /api/students`:

```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "course": "Computer Science"
}
```

## ⚠️ Notes

✅ Ensure MongoDB is running and the `MONGO_URI` is valid.

✅ Use tools like **Postman** or **cURL** to test API endpoints.

## 📄 License

This project is licensed under the MIT License.
