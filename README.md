<h1 align="center">🎬 DevTube</h1>

<p align="center">
  <b>A Scalable Full-Stack Video Streaming Platform Inspired by YouTube</b><br/>
  Upload, stream, comment, subscribe, and manage content just like on YouTube — now with real-time magic and scalable infrastructure.
</p>

<p align="center">
  <img src="https://img.shields.io/github/languages/top/yourusername/DevTube?color=blue" />
  <img src="https://img.shields.io/github/license/yourusername/DevTube" />
  <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg" />
</p>

---

## 🔥 Features

- 🔐 **Google OAuth 2.0 + JWT Authentication**
- 🎥 **Video Uploads via BunnyCDN + TUS**
- 📡 **Live Real-Time Updates via Socket.io**
- 💬 **Like/Dislike Videos & Comments**
- 📺 **Subscribe/Unsubscribe to Channels**
- 💾 **Secure File Storage using ImageKit & Multer**
- 🚀 **RESTful API with Express.js**
- ⚙️ **Webhooks for Video Processing Status**
- 🧠 **Modular Code Structure with Clean MVC**

---

## 🛠️ Tech Stack

| Area | Technologies |
|------|--------------|
| **Backend** | Node.js, Express.js, MongoDB, Socket.io |
| **Authentication** | Google OAuth, JWT, bcrypt.js |
| **Security** | Helmet.js |
| **File Uploads** | Multer, ImageKit |
| **Video Streaming** | BunnyCDN with TUS Protocol |
| **Real-Time** | Socket.io, Webhooks |
| **Deployment** | Railway/Render/AWS |
| **Database** | MongoDB Atlas |

---

## 🧩 Architecture Overview

```text
Client Request → Express.js Routes → Controllers → MongoDB (via Mongoose)
         ↳ Video Uploads → BunnyCDN
         ↳ Webhooks (status updates)
         ↳ Socket.io (live likes/comments)
