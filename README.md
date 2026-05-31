[English](README.md) | [Deutsch](README.de.md)

# Green Link 🌱

**Smart Dual-Zone IoT Garden Watering System**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PlatformIO](https://img.shields.io/badge/PlatformIO-ESP32-blue)](https://platformio.org/)
[![Android](https://img.shields.io/badge/Android-Jetpack%20Compose-green)](https://developer.android.com/jetpack/compose)

Green Link is an open-source, autonomous IoT irrigation system designed for efficient and precise garden watering. It combines reliable ESP32-based hardware with a modern Android application, enabling both scheduled autonomous operation and convenient remote control via WiFi.

---

## ✨ Key Features

- **Two independent watering channels** with individual control
- **PWM-based flow control** for precise watering intensity
- **Sensor integration**:
  - Capacitive soil moisture sensors (one per zone)
  - Water tank level sensor
- **DS3231 Real-Time Clock (RTC)** for accurate time-based scheduling
- **Autonomous operation** – works independently of the mobile app
- **Local WiFi communication** – no cloud service required
- **Buzzer alerts** for low water level and system notifications
- **Modern Android App** with clean Jetpack Compose UI

---

## 🛠️ Tech Stack

### Hardware & Firmware
- **Microcontroller**: ESP32
- **Framework**: PlatformIO + C++
- **Communication**: JSON over HTTP (AsyncWebServer)
- **Storage**: LittleFS + Preferences
- **Sensors & Actuators**: Soil moisture, ultrasonic/float level, PWM pumps, buzzer, DS3231 RTC

### Android Application
- **Language**: Kotlin
- **UI**: Jetpack Compose + Material 3
- **Architecture**: MVVM + Repository Pattern
- **Networking**: Ktor Client (or Retrofit)
- **Dependency Injection**: Hilt

---

## 📱 Android App Features

- Real-time sensor dashboard (humidity + water level)
- Manual pump control with PWM flow sliders
- Advanced scheduling system (per channel, recurring)
- WiFi device connection and discovery
- Responsive and intuitive user interface

---

## 📂 Project Structure

- `/firmware` – ESP32 source code
- `/android` – Jetpack Compose Android app
- `/hardware` – Schematics, BOM, and 3D models
- `/docs` – Detailed documentation and API specification

---

## 🚀 Getting Started

### Prerequisites
- ESP32 development board
- Two 12V water pumps
- Soil moisture sensors + water level sensor
- DS3231 RTC module
- Android device (API 24+)

### Firmware Setup
1. Clone the repository
2. Open the `firmware` folder in PlatformIO
3. Configure WiFi credentials in `config.h`
4. Build and flash to ESP32

### Android App Setup
1. Open the `android` folder in Android Studio
2. Connect to the same WiFi network as the device
3. Enter device IP or use discovery feature

Detailed setup instructions are available in the [docs](/docs) folder.

---

## 📸 Screenshots

*(Add screenshots here: Dashboard, Schedule screen, Manual control, Hardware photo)*

---

## 🎯 Project Goals

This project showcases full-stack IoT development skills, including embedded systems programming, hardware integration, sensor-actuator control, and modern mobile application development. It is built with clean code, modularity, and reliability in mind.

Ideal for learning or as a practical demonstration of embedded + mobile engineering capabilities.

---

## 📄 License

This project is licensed under the **MIT License** – see the [LICENSE](LICENSE) file for details.

---

## 🤝 Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

---

**Made with ❤️ by farzad for efficient and sustainable gardening.**

*Project developed as a complete IoT solution for portfolio and learning purposes.*