# 🚨 Smart Disaster Distress & Responder Routing System

A Flutter-based mobile application that enables people to send distress signals during disasters and helps nearby responders reach victims efficiently using custom-built algorithms and real-time synchronization.

---

## 📌 Overview

During disaster situations, delays in communication and poor coordination can cost lives.  
This application provides a real-time system where:

- Users can send distress signals with their live location
- Nearby responders receive alerts instantly
- Responders are prioritized using a custom algorithm
- The shortest path to the victim is calculated using a routing algorithm implemented from scratch

The project focuses on **algorithmic problem-solving**, **real-time multi-device interaction**, and **clean application architecture**.

---

## 🚀 Features

### User Side
- Send distress signal with live location
- Cancel distress within a defined time window
- Automatic distress escalation if the user becomes inactive
- Speed dial emergency contacts
- Notify friends or trusted contacts

### Responder Side
- Receive real-time distress notifications
- View prioritized distress requests
- Accept or decline requests
- Navigate to the victim using the shortest route

### System Features
- Real-time synchronization across multiple devices
- Push notifications using Firebase Cloud Messaging (FCM)
- Simulation mode for testing and demonstration
- Partial offline support for safe demo scenarios

---

## 🧠 Algorithms Implemented

### 1. Responder Prioritization Algorithm
Implemented from scratch in **pure Dart**.

**Factors considered:**
- Distance to victim
- Responder availability
- Distress urgency
- Auto-trigger timeout status

**Output:**  
A ranked list of responders based on priority.

---

### 2. Shortest Path Routing Algorithm
Implemented from scratch in **pure Dart**.

- Uses **Dijkstra or A*** algorithm
- Graph-based routing model
- Weighted edges (distance, risk, blockage)

> Maps are used only for visualization. Routing logic is fully custom.

---

## 🛠 Tech Stack

- **Flutter** – Mobile UI
- **Dart** – Core logic & algorithms
- **Firebase**
  - Firestore / Realtime Database – Real-time data sync
  - Firebase Cloud Messaging (FCM) – Push notifications
- **Maps API** – Location display and route visualization

---

## 🧩 State Management

- **GetX**

Chosen for simplicity, faster development, and controller-based separation of concerns.

---

## 🏗 Project Architecture (Mid-Level Layered)


### Architecture Principles
- Algorithms are independent of UI and Firebase
- Controllers coordinate data flow
- UI contains no business logic
- Firebase is used only for communication and storage

---

## ☁ Firebase Usage

Firebase is used strictly as a **real-time communication layer**.

It handles:
- Distress signal storage
- Responder status updates
- Real-time synchronization
- Push notifications

All decision-making logic resides in Dart algorithms.

---

## 🗺 Maps & Location

Maps are used only for:
- Displaying user and responder locations
- Visualizing routes returned by the routing algorithm

No built-in map routing logic is used.

---

## 🧪 Simulation & Demo

- Multi-device demo supported via Firebase
- Simulation mode for controlled testing
- Designed to work reliably during live demonstrations

---

## 👥 Team Roles

- **Member 1**
  - System architecture
  - Algorithm design & implementation
  - Firebase integration
  - Documentation

- **Member 2**
  - User-side Flutter UI

- **Member 3**
  - Responder-side Flutter UI

---

## 📂 Project Status

- Requirements finalized
- Architecture locked
- Core algorithms defined
- Implementation in progress

---

## 📄 License

This project is developed as part of an academic final year project.
