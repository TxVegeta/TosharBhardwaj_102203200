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

## 📸 Screenshots

### 🏠 Home Page
<img width="1447" height="796" alt="Image" src="https://github.com/user-attachments/assets/60a69e48-a83a-4eeb-aefc-aa594ee36ceb" />

### 🔗 Joining a Meeting
1. Open the app in another browser tab or device.  
2. Click **“Join Call”** on the home page.  
3. Paste the **Meeting ID** shared by the host.  
4. Click **“Join Meeting”**.  
5. You’ll immediately connect with the host via a **peer-to-peer WebRTC connection** for video, audio, and chat.
<img width="1447" height="796" alt="Image" src="https://github.com/user-attachments/assets/08a333e2-9145-4f04-8e82-0e2164697f82" />

### 💬 Chatting During the Call
-Use the **chat panel** on the right-hand side to send and receive messages.  
-Messages are transmitted in real time using **WebRTC data channels**

<img width="1470" height="835" alt="Image" src="https://github.com/user-attachments/assets/8a5b51b1-db92-459a-8c42-ac0f1561677d" />


### 🖥️ Screen Sharing
- Click the **“Share Screen”** button during a call.  
- Choose to share your **entire screen**, a **specific window**, or a **browser tab**.  
- Your peer will immediately see the shared content in real-time.
  
<img width="1470" height="835" alt="Image" src="https://github.com/user-attachments/assets/7adaffd0-050a-4d5c-8382-cf3af14622ae" />
