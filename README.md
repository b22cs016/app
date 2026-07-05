# Real-Time Chat Application

A lightweight, real-time chat application built using **Spring Boot**, **Java WebSockets (STOMP)**, and a **Thymeleaf** frontend stylized with Bootstrap. 

This application sets up a seamless, two-way communication channel between multiple clients, allowing users to join a shared chat room and exchange messages instantly without requiring any page refreshes.

---

## 🚀 Features

*   **Real-Time Bi-directional Communication:** Instant text delivery across all connected browser windows using WebSockets.
*   **STOMP Protocol over SockJS:** Built-in protocol abstraction with robust fallback behaviors for networks or older browsers lacking pure WebSocket support.
*   **Dynamic Chat UI:** Scroll-optimized chat logs and responsive message styling powered by Bootstrap.
*   **Persistent User Session:** Tracks sender identities in the browser view dynamically without clearing user handles between sent messages.

---

## 🛠️ Technology Stack

### Backend
*   **Java 17+**
*   **Spring Boot:** Core backend framework.
*   **Spring WebSocket & Messaging:** Powers live messaging capabilities.
*   **STOMP (Simple Text Oriented Messaging Protocol):** Organizes, routes, and broadcasts room subscriptions.
*   **Lombok:** Minimizes boilerplate code for data models.

### Frontend
*   **Thymeleaf:** Server-side templating engine to bind HTML views.
*   **JavaScript (ES6):** Handles client-side socket connection states and DOM updates.
*   **SockJS-client & Stomp-client:** Handles the connection pipeline and broker subscriptions.
*   **Bootstrap 5:** Clean, responsive interface layout.

### Build Tools
*   **Maven**

---

## 📂 Architecture & Endpoint Design

The application routes client payloads through an in-memory message broker.
