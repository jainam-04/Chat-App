# 💬 Real-Time Chat Application

A real-time chat application built using **Spring Boot**, **WebSockets**, **SockJS**, and **STOMP.js**.  
It supports multiple users chatting simultaneously with instant message delivery via WebSocket-based communication.

---

## 🧭 Table of Contents

- [🚀 Features](#-features)  
- [🏗️ Tech Stack](#️-tech-stack)
- [⚙️ Setup and Run](#️-setup-and-run)
- [🧰 Dependencies](#-dependencies)
- [📸 Screenshot](#-screenshot)
- [🧠 How It Works](#-how-it-works)
- [📧 Contact](#-contact)

---

## 🚀 Features

- 🔄 Real-time messaging using **WebSockets**
- 🧑‍🤝‍🧑 Support for multiple users and chat rooms
- 💡 SockJS fallback for browsers that don’t support native WebSockets
- 🗣️ STOMP protocol for structured message communication
- 📡 Backend built with **Spring Boot**
- 🌐 Frontend integrated with **STOMP.js**
- ⚙️ Simple REST APIs for user management (optional)

---

## 🏗️ Tech Stack

| Layer | Technology |
|-------|-------------|
| Backend | Spring Boot, Spring WebSocket |
| Protocol | STOMP (Simple Text Oriented Messaging Protocol) |
| WebSocket Fallback | SockJS |
| Frontend | JavaScript (STOMP.js) |
| Build Tool | Maven / Gradle |

---


## ⚙️ Setup and Run

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/jainam-04/Chat-App.git
cd spring-boot-chat-app
```
### 2️⃣ Build the Application
```bash
mvn clean install
```
### 3️⃣ Run the Application
```bash
mvn spring-boot:run
```
### 4️⃣ Access the App
```bash
http://localhost:8080/
```

---

## 🧰 Dependencies

- Spring Boot Starter Web
- Spring Boot Starter Thymeleaf
- Lombok
- Spring Boot Starter Websocket

## 📸 Screenshot

![WhatsApp Image 2025-10-30 at 20 29 06_c879d706](https://github.com/user-attachments/assets/6f84c274-749f-41a7-a6c2-5de1409af410)

---

## 🧠 How It Works

1. Client connects to the WebSocket endpoint /ws using SockJS.
2. STOMP protocol is used to send and receive structured messages.
3. Messages are routed through Spring’s @MessageMapping methods.
4. The broker broadcasts messages to all subscribers on the topic (e.g., /topic/public).

---

## 📧 Contact

If you have any questions or suggestions, feel free to reach out:
Jainam Rupani – jainamrupani04@gmail.com
