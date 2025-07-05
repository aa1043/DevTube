<h1 align="center">🎬 DevTube</h1>

<p align="center">
  A Scalable Full-Stack Video Streaming Platform Inspired by YouTube  
  <br>
  Upload, stream, comment, subscribe, and manage content — just like on YouTube — with real-time magic and scalable infrastructure.
</p>

<p align="center">
  <img src="https://img.shields.io/github/languages/top/aa1043/DevTube?color=blue" />
  <img src="https://img.shields.io/github/license/aa1043/DevTube" />
  <img src="https://img.shields.io/github/issues-pr/aa1043/DevTube?label=PRs" />
  <img src="https://img.shields.io/badge/status-active-success" />
</p>

---

## 📚 Table of Contents

- [✨ Features](#-features)
- [🧩 Tech Stack](#-tech-stack)
- [⚙️ Architecture Overview](#️-architecture-overview)
- [🚀 Getting Started](#-getting-started)
- [🙌 Acknowledgements](#-acknowledgements)

---

## ✨ Features

- 🎥 **Video Upload & Streaming** — Upload and watch HD videos.
- 💬 **Commenting System** — Real-time user interactions.
- 📺 **Channel Management** — Create & customize your own channel.
- 🧠 **Smart Tag Search** — Discover videos by hashtags.
- 📊 **Studio Dashboard** — Monitor views, subscribers, and analytics.
- 🔒 **OAuth Authentication** — Secured login and user data.

---

## 🧩 Tech Stack

| Category      | Tech                              |
|---------------|-----------------------------------|
| Frontend      | HTML, CSS, JavaScript, EJS        |
| Backend       | Node.js, Express.js               |
| Database      | MongoDB, Mongoose                 |
| Auth          | OAuth                             |
| Realtime      | Socket.io                         |
| Video CDN     | BunnyCDN                          |

---

## ⚙️ Architecture Overview

```text
Client Request → Express.js Routes → Controllers → MongoDB (via Mongoose)
         ↳ Video Uploads → BunnyCDN
         ↳ Webhooks → Update DB
         ↳ Socket.io → Live likes/comments
