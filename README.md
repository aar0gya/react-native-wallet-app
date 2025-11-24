# 💰 React Native Wallet App

A full-stack personal finance wallet mobile application built with **React Native (Expo), Express.js, PostgreSQL (Neon), Redis, and Clerk authentication**. This app lets users safely manage personal transactions with real backend storage, live syncing, and secure login.

---

## 🚀 Features

### 🔐 Authentication

* Email sign-in using Clerk
* 6-digit verification code flow
* Secure token-based authentication

### 📱 Mobile App

* Works on **iOS & Android**
* Beautiful home screen displaying:

  * Current balance
  * Past transactions
* Create a screen for adding:

  * Income transactions
  * Expense transactions
* Swipe down to pull-to-refresh
* Delete transactions and dynamically update the balance
* Logout returns the user to the login screen

### 🧠 Backend

* Express REST API
* PostgreSQL database hosted on Neon
* Clerk middleware for validating user tokens
* Redis for API rate limiting

---

## 🧰 Tech Stack

| Category             | Technology                           |
| -------------------- | ------------------------------------ |
| Mobile               | React Native, Expo, React Navigation |
| Backend              | Node.js, Express                     |
| Authentication       | Clerk                                |
| Database             | PostgreSQL (Neon)                    |
| Caching / Rate Limit | Redis                                |
| Deployment           | Cloud-based hosting                  |

---

## 📸 Screenshots

> *(Add images here when uploading to repo)*

Example (image):

```
/assets/screens/home.png
/assets/screens/login.png
/assets/screens/create.png
```

---

## ⚙️ Environment Setup

### Backend `.env`

```
PORT=5001
NODE_ENV=development

CLERK_PUBLISHABLE_KEY=<your_clerk_publishable_key>
CLERK_SECRET_KEY=<your_clerk_secret_key>

DATABASE_URL=<your_neon_postgres_connection_url>
REDIS_URL=<your_redis_connection_url>
```

### Mobile `.env`

```
EXPO_PUBLIC_CLERK_PUBLISHABLE_KEY=<your_clerk_key>
```

---

## 🛠 Running the Project

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

Use a real device or simulator to test the app.

---

## 📚 What You'll Learn

* Build and deploy a full Express API
* Integrate Clerk authentication with email verification
* Store data in a real PostgreSQL cloud database
* Connect mobile UI to backend services
* Implement rate limiting with Redis
* Deploy mobile and server applications
* Understand React Native navigation and state management

---

## 📝 Folder Structure

```
root
│
├── backend
│   ├── src
│   ├── package.json
│   ├── .env
│
└── mobile
    ├── App.js
    ├── screens/
    ├── components/
    ├── .env
```

---

## 🧾 License

This project is licensed under the MIT License — see `LICENSE` for details.

---

## ⭐ Contribute

Pull requests and feature contributions are welcome! Feel free to open an issue for suggestions or bugs.

---

## 📩 Contact

If you have questions or want help extending the app, feel free to ask!

Happy coding 🎉
