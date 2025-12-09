# 🍕 Real-Time Pizza Ordering App (MERN + Socket.IO)

A full-stack real-time pizza ordering web application built using **MongoDB, Express, React, Node.js, and Socket.IO**.  
Users can place orders, track status live without refreshing, and admins can manage and update order states in real time.

---

## 🚀 Features

### 👤 User
- Register and login using JWT authentication
- Browse pizza menu
- Add items to cart and checkout
- Track order status **live** (Placed → Baking → Out for Delivery → Delivered)

### 🛠 Admin
- View all customer orders
- Update order status in real-time
- Manage pizza inventory

### ⚡ Real-Time
- WebSocket-powered live order updates using **Socket.IO**
- No refresh needed to see order progress

---

## 🧩 Tech Stack

| Layer | Technology |
|-------|------------|
| Frontend | React.js, Context API/Redux, Axios, Tailwind/Bootstrap |
| Backend | Node.js, Express.js |
| Database | MongoDB + Mongoose |
| Real-Time | Socket.IO |
| Auth | JWT + bcrypt |

---

## 📂 Project Structure

/client --> React frontend
/server --> Node.js + Express backend
/models --> MongoDB schemas
/controllers --> Business logic
/routes --> API endpoints

yaml
Copy code

---

## 🛠 Setup Instructions

### 1️⃣ Clone Repository
```sh
git clone https://github.com/yourusername/real-time-pizza-app.git
cd real-time-pizza-app
2️⃣ Install Dependencies
Backend:

sh
Copy code
cd server
npm install
Frontend:

sh
Copy code
cd client
npm install
3️⃣ Environment Variables
Create .env in /server:

ini
Copy code
MONGO_URI=your_mongodb_url
JWT_SECRET=your_secret
PORT=5000
4️⃣ Run App
Backend:

sh
Copy code
npm start
Frontend:

sh
Copy code
npm start
🔄 Real-Time Flow
User places order → stored in MongoDB

Admin sees new order instantly

When admin updates status → Socket.IO broadcasts update

Customer UI updates without refreshing