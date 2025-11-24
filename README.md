# 💰 React Native Wallet App

A full-stack personal finance wallet application built using **React Native, Expo, Express, Clerk, Neon PostgreSQL, and Redis**.
This project demonstrates how to build a complete production-ready mobile application with **authentication, database integration, cloud deployment, and real-time updates** — all without needing Swift, Kotlin, or native modules.

This project demonstrates how to build a fully functional, production-ready mobile finance tracker using React Native + Expo alongside a Node.js/Express backend with:

⦁	Clerk authentication (with email code verification)

⦁	Neon PostgreSQL for database storage

⦁	Redis rate limiting

⦁	Deployed backend and real device mobile support

Users can:

⦁	Sign up & log in using a 6-digit email code

⦁	View their current wallet balance

⦁	Create income or expense transactions

⦁	Delete transactions, with recalculations

⦁	Pull-to-refresh to sync with backend

⦁	Log out securely

Perfect for developers looking to learn how to connect a mobile frontend to a real backend with secure user accounts and persistent cloud data storage.

---

## 🚀 Features

### ✨ Mobile App (Expo & React Native)

* 📱 Runs on **iOS & Android**
* 🔐 Email-based login & signup (6-digit verification code) using Clerk
* 💼 Home screen showing:

  * Current balance
  * List of transactions
* ➕ Add income and expense transactions
* 🔄 Pull-to-refresh functionality
* ❌ Delete transactions to update balance instantly
* 🚪 Logout routing that safely returns users to auth pages

### 🖥 Backend (Express API)

* 🌐 Fully REST-based Node.js server
* 🗄 PostgreSQL database hosted on Neon
* ⚙ Auth middleware using Clerk
* 📦 Redis-based rate limiting for protection
* ☁ Easily deployable on cloud services

---

## 🧠 What You'll Learn

By building this project, you’ll master:

* Building a **mobile app with React Native & Expo**
* Creating a **backend with Express & PostgreSQL**
* Real-world user authentication with **Clerk**
* Structured full-stack communication between mobile → backend → database
* Implementing rate limiting using **Redis**
* Deployment of both backend & mobile applications
* Managing navigation & global app state cleanly

Perfect for:

* Beginners building their *first full-stack mobile app*
* React developers expanding into React Native
* Anyone needing a realistic production-ready example

---


## 📸 App Screenshots

<p align="center">
  ![Screenshot_2025-11-24-17-34-06-40_f73b71075b1de7323614b647fe394240](https://github.com/user-attachments/assets/bd44a4ec-c9b6-48cd-a210-76cbfba1c212)
</p>

---

## 🛠 Tech Stack

### Frontend

* React Native (Expo)
* React Navigation
* Async Storage
* Clerk Auth SDK

### Backend

* Node.js + Express
* PostgreSQL (Neon)
* Redis (Rate Limiting)
* Clerk Server SDK

---

## 📁 Project Structure

```
.
├── backend
│   ├── src
│   ├── package.json
│   └── .env
└── mobile
    ├── screens
    ├── components
    ├── package.json
    └── app.config.js
```

---

## ⚙ Environment Variables

### Backend (`/backend/.env`)

```
PORT=5001
NODE_ENV=development

CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>

DATABASE_URL=<your_neon_postgres_connection_url>
REDIS_URL=<your_redis_connection_url>
```

### Mobile (`/mobile/.env`)

```
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=<your_clerk_key>
```

---

## ▶ Running The Project

### 1️⃣ Start Backend

```bash
cd backend
npm install
npm run dev
```

### 2️⃣ Start Mobile App

```bash
cd mobile
npm install
npx expo start
```

Scan the QR code or run the Android/iOS simulator.

---

## 📡 Deployment

You can deploy using:

### Backend:

* Vercel
* Render
* Fly.io
* Railway

### Database:

* Neon PostgreSQL (recommended)

### Redis:

* Upstash (free tiers available)

### Mobile:

* Expo EAS (supports OTA & store publishing)

---

## 📌 Roadmap

* [ ] Dark mode UI
* [ ] Filtering & sorting transactions
* [ ] Budget goals overview
* [ ] Push notifications for expenses

---

## 🧾 License

This project is open-source — see `LICENSE` for details.

---

## ⭐ Support

If this project helps you:

* Star ⭐ the repository
* Share with developers getting into React Native

## 🧾 Note
This backend is an API server. Opening the Render URL in a browser will not show a webpage — it is meant to serve the mobile app. If you open it directly, you may see “Cannot GET /”.

Thanks,
Happy coding!
aar0gya
