# 🚌 Online Bus Ticket Reservation System

**Developer: Muhammad Ismail**

A complete full-stack web project where users can search buses, book tickets, send feedback, and contact admin.
Admins can manage buses, routes, schedules, bookings, feedback, and contact messages through a dedicated admin panel.

---

## 🚀 Features

### **User Features**

* Search buses by **From**, **To**, **Date**, **Passengers**
* View full bus details (time, duration, price, seat type)
* Book bus tickets online
* Contact form (message sent to admin)
* Feedback system (rating + comments)
* Fully responsive UI

### **Admin Features**

* Secure admin login
* Add / Update:

  * Cities
  * Routes
  * Buses
  * Schedules
* View all bookings
* View and reply to contact messages
* View customer feedback
* Dashboard-style layout

---

## 🛠 Tech Stack

### **Frontend**

* React (TypeScript)
* Vite
* TailwindCSS

### **Backend**

* Node.js
* Express.js
* MySQL (mysql2)

### **Database Tables**

* `cities`
* `routes`
* `buses`
* `schedules`
* `bookings`
* `contact_messages`
* `feedback`

---

## 📂 Project Structure

```
project/
│
├── client/                # React Frontend
│   ├── src/pages
│   ├── src/components
│   └── index.html
│
├── server/                # Node.js Backend
│   ├── routes
│   ├── db.ts
│   ├── index.ts
│   └── schema.sql
│
└── package.json
```

---

## ⚙️ Installation Guide

### **1. Clone the Project**

```bash
git clone https://github.com/your-username/online-bus-reservation.git
cd online-bus-reservation
```

---

## 🔧 Backend Setup

### **2. Install Dependencies**

```bash
pnpm install
```

---

### **3. Import Database Schema**

In MySQL / phpMyAdmin:

```sql
SOURCE server/schema.sql;
```

---

### **4. Create Backend `.env` File (`server/.env`)**

```
DB_HOST=localhost
DB_USER=root
DB_PASS=
DB_NAME=bus_reservation
PORT=3000
CORS_ORIGIN=*
```

---

### **5. Start Backend**

```bash
pnpm build
pnpm start
```

Backend runs at:

👉 **[http://localhost:3000](http://localhost:3000)**

---

## 🌐 Frontend Setup

### **6. Install Frontend Dependencies**

```bash
cd client
pnpm install
```

---

### **7. Create Frontend `.env` (`client/.env`)**

```
VITE_API_BASE_URL=http://localhost:3000
```

---

### **8. Start Frontend**

```bash
pnpm dev
```

Frontend runs at:

👉 **[http://localhost:5173](http://localhost:5173)**

---

## 🔐 Admin Login (Default)

```
Phone/Email: 03001234567
Password: Admin@123
```

---

## 📩 Contact Messages

Users send messages using the Contact form.
Admin can view and reply.

Stored in MySQL table:

```
contact_messages
```

---

## ⭐ Feedback System

Users can submit:

* ⭐ Ratings
* 💬 Comments

Admin can view all feedback.

Stored in:

```
feedback
```

---

## 📦 Build for Production

```bash
pnpm build
```

---

## 👨‍💻 Developer

**Muhammad Ismail**

---

## 🤝 Contributing

Pull requests are welcome.
For major changes, open an issue first.

---

## 📄 License

MIT License © 2025 Muhammad Ismail

