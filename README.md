<h1 align="center">🎬 DevTube</h1>

<p align="center">
  A Scalable Full-Stack Video Streaming Platform Inspired by YouTube  
  <br>
  Upload, stream, comment, subscribe, and manage content — just like on YouTube — now with real-time magic and scalable infrastructure.
</p>

<p align="center">
  <img src="https://img.shields.io/github/languages/top/aa1043/DevTube?color=blue" />
  <img src="https://img.shields.io/github/license/aa1043/DevTube" />
  <img src="https://img.shields.io/github/issues-pr/aa1043/DevTube?label=PRs" />
  <img src="https://img.shields.io/badge/status-active-success" />
</p>

---

## 📽️ Demo

> Coming soon — stay tuned! (Or embed your video link here if you have one)

---

## ✨ Features

- 🎥 **Video Upload & Streaming**  
  Upload videos and stream them directly from the platform.

- 💬 **Comments & Replies**  
  Engage users with threaded commenting.

- 📺 **Channel System**  
  Each user can create and manage a personal channel.

- 🧠 **Hashtags & Search**  
  Discover content using tags and keywords.

- 🧾 **Studio Dashboard**  
  Customize channel, view analytics, manage content.

- 🧱 **Modular Architecture**  
  Built with a scalable and clean folder structure.

---

## 🧩 Tech Stack

| Category      | Tech                              |
|---------------|-----------------------------------|
| Frontend      | HTML, CSS, JavaScript, EJS        |
| Backend       | Node.js, Express.js               |
| Database      | MongoDB, Mongoose                 |
| Auth          | OAuth                             |
| UI Frameworks | Custom CSS                        |

---

## 🧩 Architecture Overview

```text
Client Request → Express.js Routes → Controllers → MongoDB (via Mongoose)
         ↳ Video Uploads → BunnyCDN
         ↳ Webhooks (status updates)
         ↳ Socket.io (live likes/comments)
