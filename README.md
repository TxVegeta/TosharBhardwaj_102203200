# 🎥 VidConnect 🚀  
**VidConnect** is a real-time, peer-to-peer video calling application built with modern web technologies.  
It allows users to create unique meeting rooms and connect directly for **low-latency video, audio, and chat** communication.

---

## ✨ Key Features

- 🎦 **Real-time Video & Audio** — High-quality, low-latency streaming powered by WebRTC  
- 💬 **Live Text Chat** — A dedicated chat panel for messaging during the call  
- 🖥️ **Screen Sharing** — Share your screen or a specific application window with your peer  
- 🔗 **Multi-Meeting Support** — Create and join distinct, isolated meetings with unique IDs  
- 🔔 **Graceful Disconnects** — Users are instantly notified when a peer leaves the call  

---

## 🛠️ Tech Stack

| Layer | Technologies |
|--------|---------------|
| **Frontend** | React, TypeScript, Tailwind CSS |
| **Backend** | Node.js, TypeScript, ws (WebSocket) |
| **Core** | WebRTC |

---

## ⚙️ Getting Started Locally

Follow these instructions to get the project running on your local machine for development and testing.

### ✅ Prerequisites

Make sure you have the following installed:
- [Node.js](https://nodejs.org/) (v18 or later)
- npm (comes with Node.js)

---

### 🧩 Installation & Setup

#### 1. Clone the Repository
```bash
git clone <your-repository-url>
cd <project-directory>
```
Running the Application

You will need two terminals — one for the backend server and one for the frontend client.

1️⃣ Start the Signaling Server (Backend)
```bash
cd backend
tsc -b
node dist/index.js
```
Your signaling server will now run at ws://localhost:8080.

2️⃣ Start the React Client (Frontend)
```bash
cd frontend
npm install
npm run dev
```
## How to Use the App 🎬
Open two separate browser tabs or windows and navigate to the application's home page (http://localhost:5173).

In the first tab:

Click on Start Call.

A unique Meeting ID will be generated. Copy this ID.

In the second tab:

Click on Join Call.

Paste the copied Meeting ID into the input field.

Click the Join Meeting button.

The two browser tabs will establish a peer-to-peer WebRTC connection. Your video call is now live!
