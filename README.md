# 🚍 Smart Campus Bus Tracking & Capacity Management System

A real-time IoT and mobile-based solution designed to improve campus transportation efficiency by providing live bus location tracking and seat availability using a Google-centric technology stack.

---

## 📖 Abstract

Efficient transportation within large university campuses is essential for reducing congestion and ensuring timely mobility. However, traditional campus transit systems lack real-time visibility and passenger capacity awareness. This project presents a Smart Campus Bus Tracking and Capacity Management System that leverages IoT hardware, Firebase Realtime Database, and a Flutter mobile application to deliver live bus location and seat availability to students. The system is scalable, cost-effective, and fully serverless, enabling seamless real-time data synchronization and improved campus transit efficiency.

---

## ✨ Features

- 📍 Real-time GPS-based bus tracking
- 🧮 Accurate seat availability using bi-directional IR sensors
- ☁️ Serverless backend using Firebase Realtime Database
- 📱 Flutter mobile application with Google Maps integration
- ⚡ Instant real-time updates without manual refresh
- 🔄 Scalable architecture for multiple buses

---

## 🏗️ System Architecture

The system is divided into three layers:

### 1️⃣ On-Bus Hardware (Edge Layer)
- **Controller:** Raspberry Pi Pico W (MicroPython)
- **GPS Module:** NEO-6M
- **Passenger Counting:** Bi-directional IR Sensors
- **Connectivity:** Campus Wi-Fi

### 2️⃣ Cloud Backend
- **Platform:** Firebase Realtime Database
- **Communication:** HTTP REST (PATCH)
- **Sync Mechanism:** Real-time WebSocket updates

### 3️⃣ Mobile Application
- **Framework:** Flutter
- **Maps:** Google Maps SDK
- **Data Handling:** StreamBuilder (real-time streams)

---

## 🔄 System Workflow

1. Raspberry Pi Pico W boots and connects to campus Wi-Fi  
2. GPS module acquires real-time location  
3. IR sensors update passenger count on entry/exit  
4. Data is transmitted to Firebase every 3–5 seconds  
5. Firebase pushes updates to connected clients  
6. Flutter app updates bus marker and seat availability live  

---

## 🧰 Technology Stack

| Layer | Technologies |
|-----|-------------|
| Hardware | Raspberry Pi Pico W, NEO-6M GPS, IR Sensors |
| Firmware | MicroPython |
| Backend | Firebase Realtime Database |
| Mobile App | Flutter, Google Maps SDK |

---

## campus-bus-tracker
├── hardware/ # IoT firmware & hardware setup
├── cloud/ # Firebase schema & rules
├── mobile_app/ # Flutter application


---

### Hardware Setup
1. Connect GPS and IR sensors to Raspberry Pi Pico W
2. Flash MicroPython firmware
3. Configure Wi-Fi and Firebase credentials

### Firebase
- Create a Firebase Realtime Database
- Update database rules and schema from `/cloud`


## 👥 Team

Team Name: Alpha Hackers

- Sivashankari V
- Sri Vaishnavi Karthika K
- Veronica S
- Sri Balaji Raja S
DEPARTMENT OF INFORMATION TECHNOLOGY
PSNA COLLEGE OF ENGINEERING AND TECHNOLOGY
