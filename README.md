# 📱 Mini Social Media Platform

A full-stack **Mini Social Media Application** that enables users to connect, share content, and interact with each other through posts, comments, likes, and follows. This project demonstrates core concepts of modern web development including frontend UI design, backend APIs, and database management.

---

## 📌 Project Overview

This application simulates a simplified version of real-world social media platforms. Users can create accounts, share posts, interact with other users, and build a social network.

The goal of this project is to understand:

* Full-stack architecture
* REST API design
* User interaction systems
* Database relationships

---

## 🚀 Key Features

### 👤 User Management

* User registration & login
* Profile creation and updates
* View other user profiles

### 📝 Post System

* Create, edit, delete posts
* Each post linked to a user
* Timestamp for every post

### 💬 Comment System

* Add comments to posts
* View all comments per post
* Nested or simple comment structure

### ❤️ Like System

* Like/unlike posts
* Like count display
* Prevent duplicate likes

### 👥 Follow System

* Follow/unfollow users
* Followers & following count
* Personalized user feed (optional)

---

## 🛠️ Tech Stack

### Frontend

* HTML5 – Structure
* CSS3 – Styling & Layout
* JavaScript – Interactivity & DOM manipulation

### Backend (Choose One)

* **Django (Python)** – MVT architecture, built-in admin panel
  **OR**
* **Express.js (Node.js)** – Lightweight REST API framework

### Database

* SQLite / MongoDB / MySQL

---

## 🧠 System Architecture

```id="arch1"
/Client (Frontend)
        ↓
REST API (Backend Server)
        ↓
Database (Users, Posts, Comments, Followers)
```

---

## 🗂️ Database Design

### Users Table

* id (Primary Key)
* username
* email
* password (hashed)
* profile_picture
* bio

### Posts Table

* id
* user_id (Foreign Key)
* content
* created_at

### Comments Table

* id
* post_id (Foreign Key)
* user_id (Foreign Key)
* comment_text
* created_at

### Followers Table

* id
* follower_id
* following_id

### Likes Table

* id
* user_id
* post_id

---

## 📂 Folder Structure

```id="struct1"
/mini-social-media
│
├── frontend/
│   ├── index.html
│   ├── profile.html
│   ├── style.css
│   ├── script.js
│
├── backend/
│   ├── server.js / app.py
│   ├── routes/
│   ├── controllers/
│   ├── models/
│
├── database/
│   └── schema.sql / models.py
│
├── assets/
│   └── images/
│
└── README.md
```

---

## ⚙️ Installation Guide

### 1️⃣ Clone Repository

```
git clone https://github.com/your-username/mini-social-media.git
cd mini-social-media
```

### 2️⃣ Backend Setup

#### For Express.js

```
npm install
npm start
```

#### For Django

```
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```

---

### 3️⃣ Frontend Setup

Just open:

```
index.html
```

OR run using Live Server in VS Code.

---

## 🔌 API Endpoints (Example)

### User APIs

* `POST /register`
* `POST /login`
* `GET /users/:id`

### Post APIs

* `GET /posts`
* `POST /posts`
* `DELETE /posts/:id`

### Comment APIs

* `POST /comments`
* `GET /comments/:postId`

### Follow APIs

* `POST /follow`
* `POST /unfollow`

---

## 🔐 Security Considerations

* Password hashing (bcrypt)
* Input validation
* Authentication (JWT/session-based)
* Prevent SQL Injection / XSS

---

## 📸 Screenshots

Example:

```
  <img width="1501" height="844" alt="image" src="https://github.com/user-attachments/assets/898df22e-f8d4-476b-b7fb-75cbbdcfb3f8" />

  <img width="1916" height="612" alt="image" src="https://github.com/user-attachments/assets/9ff7653c-408f-406b-9ab0-4739a116eb3c" />

  <img width="1913" height="691" alt="image" src="https://github.com/user-attachments/assets/77ea5df8-d7c3-4bc7-b0d1-cd8a8f124206" />

  <img width="1919" height="678" alt="image" src="https://github.com/user-attachments/assets/30374555-14a4-4129-8a62-f7e07c37c2cf" />

  <img width="926" height="550" alt="image" src="https://github.com/user-attachments/assets/a217893d-cda1-4a05-9b8d-dfe137848fd2" />

  <img width="1911" height="640" alt="image" src="https://github.com/user-attachments/assets/0ff4fe16-59c9-4183-81b6-b2ad23f8c142" />

 
```

---

## 📊 Future Enhancements

* 🔐 Authentication with JWT
* 📷 Image & video upload
* 🔔 Notifications system
* 💬 Real-time chat (Socket.io / WebSockets)
* 🌙 Dark mode toggle
* 📱 Responsive mobile UI

---

## 🎯 Learning Outcomes

* Full-stack development understanding
* API integration
* Database relationship handling
* UI/UX design basics

---

## 🤝 Contribution

Contributions are welcome!

Steps:

1. Fork the repo
2. Create a new branch
3. Commit your changes
4. Open a Pull Request

---

## 📄 License

This project is developed for **educational purposes only**.

---
