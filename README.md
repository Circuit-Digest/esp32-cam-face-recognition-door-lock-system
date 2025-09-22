# ESP32-CAM Face Recognition Door Lock System  

[![Board](https://img.shields.io/badge/Board-ESP32--CAM-blue)](https://www.espressif.com/en/products/devkits/esp32-cam) 
[![Language](https://img.shields.io/badge/Language-Arduino%20C++-orange)](https://www.arduino.cc/reference/en/) 
[![Project](https://img.shields.io/badge/Project-CircuitDigest-green)](https://circuitdigest.com)  

---

## 📘 Tutorial Link  
👉 [ESP32-CAM Face Recognition Door Lock System](https://circuitdigest.com/microcontroller-projects/esp32-cam-face-recognition-door-lock-system)  

## 🔗 Project Type  
👉 [ESP32 CAM](https://circuitdigest.com/microcontroller-projects/how-to-program-esp32-cam-using-arduino)  

---

## 🖼️ Main Project Image  
![ESP32-CAM Face Recognition Door Lock System](https://circuitdigest.com/sites/default/files/projectimage_mic/ESP32-CAM-Digital-Lock-System.jpg)  

---

## 🚀 Features  
- Face Recognition–based authentication using ESP32-CAM.  
- Automatic door unlocking with solenoid lock and relay control.  
- No physical keys or RFID cards required.  
- Web-based streaming interface for live monitoring.  
- Supports multiple face enrollments.  
- Low-cost and compact design suitable for DIY security systems.  

---

## 🛠️ Hardware Requirements  

| Component        | Quantity | Description |
|------------------|----------|-------------|
| ESP32-CAM Module | 1        | AI-Thinker ESP32 with OV2640 Camera |
| FTDI Programmer  | 1        | For uploading code (USB to Serial) |
| Relay Module     | 1        | To switch the solenoid lock |
| Solenoid Lock    | 1        | 12V DC electronic lock |
| Power Supply     | 1        | 12V @ 500mA for solenoid |
| Jumper Wires     | As req.  | For connections |

---

## ⚙️ How It Works  
1. ESP32-CAM streams live video feed over Wi-Fi.  
2. User enrolls face(s) via the web interface.  
3. When a recognized face appears, ESP32 triggers the relay.  
4. Relay energizes the solenoid lock, unlocking the door for 5 seconds.  
5. After timeout, the lock automatically re-engages.  

---

## 🔌 Circuit Connection  

### Circuit Diagram  
![ESP32-CAM Face Recognition Door Lock Circuit](https://circuitdigest.com/sites/default/files/circuitdiagram_mic/Face-Recognition-Door-Lock-Circuit-Diagram.png)  

### Pin Mapping  

| ESP32-CAM | FTDI Programmer | Relay Module |
|-----------|-----------------|--------------|
| 5V        | VCC             | VCC          |
| GND       | GND             | GND          |
| UOR       | TX              | -            |
| UOT       | RX              | -            |
| IO0 → GND | Boot Mode       | -            |
| IO4       | -               | IN           |

⚠️ **Note:** Connect IO0 to GND before flashing code. Remove after programming.  

---

## 🧠 Troubleshooting  

| Issue | Possible Cause | Solution |
|-------|----------------|----------|
| Code not uploading | IO0 not grounded | Connect IO0 → GND before flashing |
| Camera not detected | Wrong board selected | Use **ESP32 Wrover Module** in Arduino IDE |
| Lock not working | Relay wiring issue | Check IN pin connection to IO4 |
| Face not recognized | Poor lighting / camera angle | Enroll face under good lighting conditions |
| ESP not starting | Insufficient power | Use stable 5V supply for ESP32-CAM |

---

## 📱 Applications  
- Smart home door locks  
- Office/Workspace access control  
- Hostel and apartment entry systems  
- Secure IoT-based automation projects  

---

## 🔮 Future Enhancements  
- Cloud-based face recognition (faster and more accurate).  
- Integration with mobile app notifications.  
- Adding keypad/RFID fallback authentication.  
- Battery backup with low-power ESP32 modes.  
- Logging entry attempts with timestamps.  

---

## 🧪 Technical Specifications  

| Parameter         | Value |
|-------------------|-------|
| Microcontroller   | ESP32-S (dual-core, LX6 CPU) |
| Camera            | OV2640 (2MP) |
| Connectivity      | Wi-Fi 802.11 b/g/n, Bluetooth |
| Relay Drive Pin   | IO4 |
| Operating Voltage | 5V (ESP32), 12V (Solenoid) |
| Lock Timeout      | ~5 seconds (configurable) |

---

## 🔗 Links  
- [ESP32-CAM Face Recognition Door Lock System](https://circuitdigest.com/microcontroller-projects/esp32-cam-face-recognition-door-lock-system)  
- [ESP32 CAM](https://circuitdigest.com/microcontroller-projects/how-to-program-esp32-cam-using-arduino)  
- [ESP32 Board Package for Arduino IDE](https://dl.espressif.com/dl/package_esp32_index.json)  
- [Arduino IDE](https://www.arduino.cc/en/software)  
- [Solenoid Lock Details](https://circuitdigest.com/microcontroller-projects/arduino-rfid-door-lock-code)  
- [ESP32-CAM Face Recognition Basics](https://circuitdigest.com/microcontroller-projects/how-to-use-esp32-camera-module-for-video-streaming-and-face-recognition)  

---

## ⭐ Support  
This is an official [CircuitDigest Project](https://circuitdigest.com).  
If you found this project helpful, consider sharing it with fellow developers and makers.  

---

## 🔖 Keywords  
`ESP32-CAM` `Face Recognition Door Lock` `Solenoid Lock` `IoT Security System` `Arduino IDE ESP32` `Relay Module` `Digital Lock Project`  
