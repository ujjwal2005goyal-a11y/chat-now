# 💬 Privacy-First Real-Time Chat Application

A full-stack **real-time chat application** built with the **MERN stack** and **WebSockets**, focused on **privacy-first communication**.  
Users can communicate **without sharing phone numbers**, making it ideal for **college groups, hostels, societies, and events**.

---

## 🌐 Live Demo

- **Website**: https://sparshsharma.vercel.app  
- **Chat App**: https://chat-mmln.onrender.com  

> ⚠️ Backend is hosted on **Render (free tier)** — first load may take **30–40 seconds** due to cold start.

---

## 📸 Preview

<img src="https://github.com/sparshsharma81/sparshsharma81/blob/main/images/11-1.gif?raw=true" width="100%" />

---

## 🎯 Problem Statement

Most messaging platforms require users to share **personal phone numbers or social profiles**, which is not suitable for privacy-conscious environments like colleges, hostels, and societies.

### Existing Limitations
- **WhatsApp** → Phone number required  
- **Telegram** → Phone number + contact notifications  
- **Instagram/Facebook** → Personal identity exposure  

### Solution
A **secure chat platform** that enables communication using **only email and password**, ensuring privacy without compromising usability.

---

## ✨ Features

### 🔐 Authentication & Security
- JWT authentication with **HTTP-only cookies**
- bcrypt password hashing (**10 salt rounds**)
- No phone number required
- Secure protected routes

### 💬 Real-Time Messaging
- WebSocket communication using **Socket.IO**
- Instant message delivery
- Online/offline user tracking
- Message persistence in MongoDB
- Optimistic UI updates

### 🖼 Media Sharing
- Image uploads via **Cloudinary**
- Supports files up to **100MB**
- CDN-optimized delivery

### 🎨 UI & UX
- Fully responsive design
- Tailwind CSS + DaisyUI
- Multiple themes (system-based)
- Loading states & skeleton loaders
- Browser notifications for new messages

### 🤖 Additional Integrations
- Google **Gemini AI** (code assistance)
- YouTube Shorts integration (no login required)
- Joke API
- Quote API
- Horoscope API
- Multiplayer **Chess game** (WebSocket-based)

---

## 🛠 Tech Stack

### Frontend
- React (Vite)
- Tailwind CSS
- DaisyUI
- Zustand (state management)
- Axios
- Socket.IO Client
- React Router DOM

### Backend
- Node.js
- Express.js
- MongoDB + Mongoose
- Socket.IO
- JWT
- bcrypt
- Cloudinary

### Deployment
- Frontend: **Vercel**
- Backend: **Render**
- Database: **MongoDB Atlas**
- Media Storage: **Cloudinary CDN**

---

## 🧩 Architecture

### Backend (MVC Pattern)
backend/
├── models/
├── controllers/
├── routes/
├── middleware/
└── lib/


### Frontend Structure
frontend/
├── pages/
├── components/
├── store/
├── api/
└── lib/




---

## 🔁 Authentication Flow

1. User registers with **name, email, password**
2. Password is hashed using bcrypt
3. User data stored in MongoDB
4. JWT token generated
5. Token sent via **HTTP-only cookie**
6. Access granted to protected routes

---

## 🔄 Real-Time Messaging Flow

1. Client connects using Socket.IO with userId
2. Server maps `userId → socketId`
3. Message sent via REST API
4. Message stored in MongoDB
5. Socket emits message to receiver
6. UI updates instantly

---

## ☁ Image Upload Flow

1. Image converted to base64 on frontend
2. Sent to backend
3. Uploaded to Cloudinary
4. Secure URL returned
5. URL stored in MongoDB

---

## 🚧 Known Limitations

- Render free tier causes cold starts
- Single profile image per user (currently)
- Group chats not implemented yet

> Cron jobs can be used to keep the backend warm.

---

## 🔮 Future Enhancements

- Read receipts & typing indicators
- Group chats
- Message editing & deletion
- Voice messages & video calls (WebRTC)
- Push notifications
- End-to-end encryption
- Mobile app (React Native)
- Desktop app (Electron)

---

## 📌 Use Cases

- College project teams
- Hostel or society communication
- Event-based group chats
- Anonymous feedback systems
- Privacy-focused communities

---

## 🎤 Elevator Pitch

A privacy-first real-time chat application built with **MERN and WebSockets**, enabling secure communication **without phone numbers**, featuring real-time messaging, media sharing, AI assistance, and production-ready deployment.

---

## 👨‍💻 Author

**Sparsh Sharma**  
Full-Stack Developer  
🌐 https://sparshsharma.vercel.app  

---

⭐ If you like this project, consider giving it a **star**!

