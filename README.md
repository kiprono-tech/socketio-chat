# 🗨️ Real-Time Chat App

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge\&logo=nodedotjs\&logoColor=white)
![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge\&logo=express\&logoColor=white)
![Socket.io](https://img.shields.io/badge/Socket.io-010101?style=for-the-badge\&logo=socketdotio\&logoColor=white)

A **real-time chat application** built using **Node.js**, **Express**, and **Socket.IO**.
It allows multiple users to join chat rooms, exchange messages instantly, and share live locations in a clean, responsive interface.

---

## 🚀 Features

* 💬 **Instant messaging** across rooms using Socket.IO
* 👥 **Room-based communication** — join specific chat rooms
* 🚫 **Profanity filtering** using the `bad-words` library
* 📍 **Share live locations** via Google Maps links
* 📱 **Responsive user interface** for all devices

---

## 🧠 Project Architecture

```
chat-app/
│
├── public/
│   ├── css/
│   │   └── styles.min.css          # Styling for chat and join pages
│   ├── js/
│   │   └── chat.js                 # Client-side logic for sockets
│   ├── chat.html                   # Main chat UI
│   └── index.html                  # Join form
│
├── src/
│   ├── utils/
│   │   ├── messages.js             # Generates message & location objects
│   │   └── users.js                # Handles user join, leave & tracking
│   └── index.js                    # Express + Socket.IO server setup
│
├── package.json
└── README.md
```

---

## 🛠️ Tech Stack

| Layer                | Technologies Used                   |
| -------------------- | ----------------------------------- |
| **Backend**          | Node.js, Express                    |
| **Real-time Engine** | Socket.IO                           |
| **Frontend**         | HTML5, CSS3, Mustache.js, Moment.js |
| **Utilities**        | bad-words, Qs                       |
| **Runtime**          | Nodemon (dev server)                |

---

## ⚙️ Installation & Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/kiprono-tech/socketio-chat.git
cd chat-app
```

### 2️⃣ Install Dependencies

```bash
npm install
```

### 3️⃣ Run the App (Development Mode)

```bash
npm run dev
```

Then visit:
👉 [http://localhost:3000](http://localhost:3000)

---

## 💡 How It Works

1. A user enters a **display name** and **room name**.
2. The server adds the user to that room.
3. Messages sent by one user are **broadcast** in real time to everyone in the room.
4. Users can click **Send Location** to share a live Google Maps link.
5. When a user disconnects, the server notifies others in the room.

---

## 📸 Screenshots *(Optional)*

```
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/3b5831ad-3fcf-4a88-89c3-8b642fd1c0e8" />
<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/0c0f22c0-63ac-498c-9a2a-5271e6e234f2" />

```

---

## 👨‍💻 Author

**Vincent Kiprono**
💼 Software Developer | 🌐 Web & Real-Time Apps Enthusiast
📧 [kiprono.tech@gmail.com](mailto:kiprono.tech@gmail.com)
🌍 [LinkedIn](https://www.linkedin.com/in/vincent-kiprono) 

---

## 🧾 License

This project is licensed under the **ISC License**.
Feel free to fork and modify for learning or personal use.

---
