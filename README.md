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
* ❌ **IR Sensor Turning Logic:** **Issue / Work in Progress.** The left/right turning logic using IR sensors (Pins A0 & A3) is currently not functioning as intended.

---

## ❓ Known Issue / Help Needed
When an object is within 20cm, the robot continues moving straight regardless of the IR sensors because the ultrasonic logic continuously overrides the left and right steering commands every loop. if any of you guys who are reading this know what to do pls feel free to give a sugesstion 

If you are contributing or reviewing this code feel free to :
1. Check the logic flow inside `void loop()`.
2. Open an **Issue** or submit a **Pull Request** if you have a solution to fix the directional steering balance.

---
                    
