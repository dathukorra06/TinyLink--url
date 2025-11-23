# 🚀 URL Shortener App

A full-stack URL Shortening application built using **EJS**, **Node.js**, **Express.js**, and **MongoDB Atlas**.  
Includes **Signup/Login**, **JWT authentication**, **bcrypt password hashing**, and a clean UI rendered with **EJS templates**.

---

## 🔗 Live Demo
👉 **Deployed Link:**  https://bitly.up.railway.app/  

---

## 📸 Screenshots

> Replace the placeholder links with your actual screenshots.

| Page | Screenshot |
|------|------------|
| Home Page | ![Home Page](./server/screenshots/homeurl.png) |
| Signup Page | ![Signup Page](./server/screenshots/signupurl.png) |
| Login Page | ![Login Page](./server/screenshots/loginurl.png) |
| Dashboard / Shortened URL View | ![Dashboard](./server/screenshots/dashboardurl.png) |

---

## 📘 Project Overview

This project allows users to generate short URLs after logging in.  
Built using **Node.js + Express**, UI in **EJS**, and database with **MongoDB Atlas**.

### ✔ Features
- 🔐 User Signup & Login with JWT  
- 🔒 Protected routes with authentication  
- 🔑 Password hashing using bcrypt  
- ✂ URL shortening with unique IDs  
- 📝 EJS template UI (home, login, signup)  
- 📦 MongoDB Atlas + Mongoose  
- 🌐 Works locally & after deployment  
- 📈 Tracking redirects (optional)

---

## ⚙️ How It Works

### 1. User Registration
- User signs up with name, email, password  
- Password hashed with bcrypt  
- JWT token created & stored in cookies  

### 2. User Login
- Password verified  
- JWT token issued  
- User redirected to **Home page**

### 3. URL Shortening
- User enters a long URL  
- Backend generates unique ID  
- Saves `{ originalUrl, shortUrl, userId }` in database  
- Shows short link: http://localhost:5000/url/abc123
- After deployment: https://bitly.up.railway.app/url/abc123
  
### 4. Redirect Logic
- Visiting the short URL redirects to original link  
- Implemented using `res.redirect()`

---

## 🛠 Tech Stack

### Frontend
- EJS Template Engine  
- HTML / CSS  

### Backend
- Node.js  
- Express.js  
- JWT Authentication  
- bcrypt  
- Cookie-parser  

### Database
- MongoDB Atlas  
- Mongoose  

---

## 📂 Project Structure

```

├── controllers/
├── middlewares/
├── models/
├── routes/
├── views/
│ ├── home.ejs
│ ├── login.ejs
│ └── signup.ejs
├── public/
├── index.js
├── package.json
└── README.md

````


---

## 🚀 Run Locally

### 1. Clone Repo
```

git clone https://github.com/prakashverma-dev/URL-Shortner-with-Analytics.git
cd URL-Shortner-with-Analytics

```

### 2. Install Dependencies 

```
npm install

```
### 3. Create .env
```
MONGO_URI=your-mongodb-atlas-url
JWT_SECRET=your-secret
PORT=5000

```

### 4. Start App

```
npm start

```


## 🤝 Contributing

Pull requests are welcome!

## ⭐ Support

**If you like this project, give it a ⭐ on GitHub!**

## 📜 License

MIT License

## 

<h3 align="center">✨ Built with love by Prakash ❤️</h3> 




