# Human Following Robot (Arduino / Adafruit Motor Shield)

An Arduino-based human-following robot code block generated via PictoBlox. The goal of this project is to use an Ultrasonic Sensor (HC-SR04) for distance control and IR sensors for directional tracking (turning left/right).

## 🛠️ Hardware Stack
* **Microcontroller:** Arduino Uno / Mega
* **Motor Driver:** Adafruit Motor Shield (`AFMotor` library)
* **Motors:** 4x DC Motors
* **Sensors:**
  * 1x Ultrasonic Sensor (Trig: Pin 15 / A1, Echo: Pin 16 / A2)
  * 2x IR Sensors (Left Pin: 14 / A0, Right Pin: 17 / A3)

---

## 🚦 Current Status
* ✅ **Ultrasonic Distance Control:** Working. The robot detects objects within 20cm, moves forward, and stops when clear.
* ❌ **IR Sensor Turning Logic:** **Issue / Work in Progress.** The left/right turning logic using IR sensors (Pins 14 & 17) is currently not functioning as intended.

---

## ❓ Known Issue / Help Needed
The current `loop()` checks the IR sensors sequentially after the distance logic, causing motor commands to immediately override each other every cycle. 

If you are contributing or reviewing this code feel free to :
1. Check the logic flow inside `void loop()`.
2. Open an **Issue** or submit a **Pull Request** if you have a solution to fix the directional steering balance.

---
