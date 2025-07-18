# Tracking and Monitoring Cattle's Health 🐄💡

This project is an IoT-based health monitoring system designed to track the vital signs and environmental conditions affecting cattle. It utilizes sensors and microcontrollers to detect parameters such as temperature, humidity, heart rate, gas levels, sound, light intensity, and more. Alerts are sent in real time via serial communication and displayed on an LCD.

## 📌 Features

- 🌡️ **Temperature and Humidity Monitoring** using DHT11 sensor
- ❤️ **Heart Rate Detection**
- 🌫️ **Gas Leak Detection**
- 🔊 **Sound Detection**
- 💡 **Light Intensity Measurement (LDR)**
- 🌱 **Soil Moisture Pump Control**
- 📺 **16x2 LCD Display Output**
- 📶 **WiFi Communication via AT Commands (ESP Module)**
- 📍 **GPS Location Extraction**
- 🚨 **Buzzer Alerts for Abnormal Conditions**
- 📡 **Real-Time Data Transmission via Serial/Network**

---

## 🛠️ Hardware Components

- Arduino UNO/Nano
- DHT11 Sensor
- IR Sensor
- Gas Sensor
- LDR (Light Dependent Resistor)
- Microphone/Sound Sensor
- Heartbeat Sensor
- GPS Module
- ESP8266 WiFi Module
- LCD 16x2 Display
- Buzzer
- Relay Module
- Water Pump
- Fan
- Power Supply (5V or 12V depending on components)

---

## ⚙️ Software Details

- **Language:** C++ (Arduino IDE)
- **Libraries Used:**
  - `LiquidCrystal.h`
  - `Wire.h`
  - `dht.h`

---

## 🚦 System Workflow

1. On boot, the system initializes sensors, LCD, and WiFi.
2. Sensors continuously collect:
   - Temperature & Humidity
   - Heartbeat data
   - Light (LDR), Gas, and Sound levels
3. Data is displayed on LCD.
4. If abnormal values are detected:
   - Fan or Pump is triggered
   - Buzzer alerts are activated
   - Data is transmitted via WiFi
5. GPS location is extracted when required.

---

## 🔧 Setup Instructions

1. Upload the Arduino code to your microcontroller.
2. Connect all the sensors to appropriate pins (as per the code).
3. Ensure the ESP module is powered and ready to accept AT commands.
4. Open Serial Monitor (9600 baud) to observe transmissions.
5. View sensor values and alerts on LCD.

---

## 📈 Sample Data Flow

```text
T:36 H:82 HB:72
L:Dark PH:7
ALERT: High Temperature!
ALERT: Cattle Detected!
