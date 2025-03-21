# IoT-Based Integration for Monitoring Real-time Health and ECG Validation

This project focuses on integrating **IoT (Internet of Things)** with **real-time health monitoring**, particularly for **ECG validation**, by leveraging wearable sensors and cloud technology. The data collected from sensors such as heart rate and body temperature are transmitted to a mobile application for display and further analysis. The project uses **Firebase** for backend support, **Flutter** for the mobile app, and **NodeMCU ESP8266** for wireless communication with the sensors.

## Project Overview

The project is designed to monitor **vital health parameters** such as:
- **Heart Rate (Pulse)** using the **MAX30102 Heart Rate Sensor**
- **Body Temperature** using the **MLX90614 Temperature Sensor**

The system continuously collects health data from the sensors, stores it in a cloud database, and displays it on a mobile app in real-time. The collected data can also trigger alert messages in case of abnormal readings.

### Key Features:
- Real-time monitoring of heart rate and body temperature.
- Data storage and retrieval via **Google Firebase**.
- Mobile app frontend built with **Flutter** for cross-platform compatibility.
- Easy user registration and login system using Firebase Authentication.
- **NodeMCU ESP8266** for wireless data transmission.

## Tech Stack
- **Flutter**: For building the mobile app interface.
- **Firebase**: For cloud database and user authentication.
- **NodeMCU ESP8266**: For wireless data transmission between sensors and mobile app.
- **Arduino IDE**: For programming the NodeMCU and interfacing with sensors.
- **MAX30102 Heart Rate Sensor**: For measuring heart rate.
- **MLX90614 Temperature Sensor**: For measuring body temperature.

## Implementation Details
### System Architecture
1. **Mobile App (Frontend)**: Developed using **Flutter** and communicates with the backend (Firebase) to display health data.
2. **Firebase (Backend)**: Provides real-time database and user authentication.
3. **IoT Sensors**: **MAX30102** and **MLX90614** sensors are used to capture health data.
4. **NodeMCU ESP8266**: Sends data from the sensors to Firebase via Wi-Fi.

### Sensors Used
- **MAX30102**: Measures heart rate using photodetectors and internal LEDs.
- **MLX90614**: Measures body temperature using infrared sensors.

## Tools Used
- **Android Studio**: For Flutter development.
- **Arduino IDE**: For programming the NodeMCU and sensors.
- **Firebase**: For user authentication and real-time data storage.

## Steps to Run the Code

### 1. Setup Firebase for Authentication and Database:
1. Go to [Firebase Console](https://console.firebase.google.com/).
2. Create a new project.
3. Set up Firebase Realtime Database and Authentication.
4. Add the Firebase configuration to your Flutter project.

### 2. Install Dependencies:
Install required packages using `flutter` for Firebase:
```bash
flutter pub add firebase_core
flutter pub add firebase_auth
flutter pub add cloud_firestore

