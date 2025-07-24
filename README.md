# MoonWalk Robotics™

> **Modular AI-Powered Humanoid Robot**
> A clean, native-coded, open-source humanoid robot project powered by ChatGPT and designed to *moonwalk* into the future.

---

## 🚀 Project Overview

MoonWalk Robotics™ is a modular humanoid robot designed with a minimalist, native-code philosophy. It combines advanced AI, precise motor control, and a sleek carbon fiber chassis to create a sci-fi-inspired robot that moves intelligently and smoothly.

The robot is controlled via a mobile/web interface and integrates ChatGPT for dynamic behavior and interaction.

---

## 🛠️ Hardware Components

### Core System

* **Dev Rig:** Alienware x16 / Razer Blade 18 (RTX 4090)
* **Robot Brain:** NVIDIA Jetson Orin Nano / Xavier NX
* **Alt Brain:** Raspberry Pi 5 (testing/fallback)
* **Storage:** 128GB SD or NVMe (\~100MB core footprint)
* **OS:** Custom Linux lite (MoonWalkOS)

### Power

* Samsung INR21700-50E Li-ion cells
* Tesla-grade 21700 backup cells
* Smart Battery Management System (BMS)
* Clean, modular wiring with hidden routing

### Motors & Movement

* Dynamixel X-series motors (XM430-W210-T)
* MG996R servos (early builds)
* Snap-fit modular joints (arms, legs, torso)
* Rubber-stabilized feet with optional pressure sensors

### Sensors

* Bosch BNO055 / MPU9250 IMU
* Gyroscope, accelerometer, compass combo for balance
* VL53L0X Time-of-Flight proximity sensors
* Optional LIDAR and force sensors

### Vision

* Intel RealSense D435 or ZED 2i primary camera
* Samsung S24 Ultra camera feed (backup)
* Image processing with OpenCV Lite (local or streamed)

### Audio

* Input: Rode smartLav or phone mic passthrough
* Output: Bone-conduction speaker or mini JBL
* Voice: Text-to-Speech + Avatar Display

### Control & Communication

* Phone link via USB/ADB or Wi-Fi tether
* Frontend dashboard (JS + Bootstrap) inspired by Diceon
* Lightweight numeric command format (no JSON bloat)
* Connectivity via Wi-Fi 6 / 5G / direct cable

### Outer Shell & Chassis

* White carbon fiber panels
* Magnetically mounted modular design
* Helmet with LED matrix or HUD display
* Neon blue LED accent strips

### 3D Printing

* Plastic prototyping with Creality Ender 3
* Final carbon fiber parts with Bambu Lab X1 Carbon or Markforged Onyx One

---

## 💻 Software Architecture

### Core Modules

* `right_arm.js`
* `left_leg.js`
* `balance.js`
* `moonwalk.js`
* `vision.js`

### Control Loop (Pseudo-code)

```js
loop() {
  readSensors()
  calculateAdjustments()
  sendMotorCommands()
  logResult()
}
```

* Inputs: sensor data
* Outputs: motor commands
* Feedback stored for auto-tuning balance, gait, and response

### Interface & Remote Control

* JS + PHP lightweight control panel
* Toggle actions, logs, feedback, overrides
* Mobile-friendly responsive layout

### Behavior Modules

* `moonwalk()` — predefined glide steps
* `celebrate()` — win animation
* `idle()` — breathing motion and standby
* `talk()` — speech or avatar emojis

### AI Brain Integration

* Powered by ChatGPT with live conversation and feedback
* Optional fallback to local small model (LLaMA3 Lite or Whisper.cpp)

### Deployment Philosophy

* Minimalist native code (\~100MB or less)
* Modular, clean, test → log → improve → repeat

---

## 📋 Roadmap

* [ ] Finalize hardware procurement
* [ ] Develop sensor reading and motor control loops
* [ ] Build remote dashboard interface
* [ ] Integrate ChatGPT behavior modules
* [ ] Prototype robot shell and mechanical joints
* [ ] Deploy and test on real hardware
* [ ] Open source all files: code, STL parts, docs

---

## 📜 License

This project is open source and licensed under the MIT License.

---

## 💙 Contact

For questions or contributions, open an issue or contact the maintainer.

---
