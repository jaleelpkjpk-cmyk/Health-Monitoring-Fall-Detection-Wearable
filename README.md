# Health Monitoring and Fall Detection Wearable

## 📌 Project Description
This project is a wearable device designed for elderly and at-risk individuals. 
It monitors heart rate (BPM) and oxygen level (SpO2) continuously. 
It also detects sudden falls using a motion sensor.

If a fall is detected or abnormal health values are found, the system sends an alert message to the caregiver using Telegram.

---

## 🎯 Aim
To improve safety for elderly people by:
- Monitoring health in real time
- Detecting accidental falls
- Sending emergency alerts instantly

---

## 🛠️ Components Used
- ESP32
- MPU6050 (for fall detection)
- MAX30102 (for BPM and SpO2)
- WiFi connection
- Telegram Bot

---

## ⚙️ How It Works

### 1️⃣ Health Monitoring
- MAX30102 sensor reads heart rate and oxygen level.
- BPM is considered valid only when IR value is greater than 5000.
- If BPM or SpO2 goes below safe level, an alert is prepared.

### 2️⃣ Fall Detection
- MPU6050 measures body movement.
- A sudden high acceleration followed by low movement is treated as a fall.

### 3️⃣ Alert System
- The device connects to WiFi.
- An emergency message is sent to the caregiver via Telegram.

---

## 🚨 Example Alert Message

EMERGENCY ALERT  
Fall Detected  
BPM: 78  
SpO2: 96%  
Please check immediately.

---

## 📸 Project Images
(Add your images here)

Example:
![Device Setup](images/setup.jpg)


---

## 💡 Features
- Real-time monitoring
- Accurate BPM validation using IR threshold
- Automatic fall detection
- Instant notification to caregiver
- Low-cost and portable design

---

## 🔮 Future Improvements
- Add GPS location tracking
- Store data in cloud
- Develop mobile application

---

## 📌 Conclusion
This project helps in monitoring health and detecting falls quickly. 
It provides safety support for elderly people and ensures quick response in emergencies.
