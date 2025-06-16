
**Next-Gen Fire Fighting Robot using Camera, Gas Sensor & SIM800L Module**
## 🔥 Next-Gen Fire Fighting Robot 🚒 
> Smart, Sensor-Based Fire Detection & Alert System
---
```markdown
 
## 📌 Table of Contents
- [🔍 Overview](#-overview)
- [🎯 Features](#-features)
- [🛠️ Tech Stack & Components Used](#️-tech-stack--components-used)
- [🧠 Working Principle](#-working-principle)
- [🖼️ Block Diagram](#-block-diagram)
- [🧪 Testing & Output](#-testing--output)
- [⚠️ Possible Challenges](#️-possible-challenges)
- [📷 Project Media](#-project-media)
- [📁 Project Structure](#-project-structure)
- [🚀 Getting Started](#-getting-started)
- [📞 Contact](#-contact)

---

## 🔍 Overview
This is a **Next-Generation Fire Fighting Robot** designed to detect fire using **flame sensors**, **gas leakage using MQ2**, provide real-time **visual feedback via an onboard camera**, and send **SMS alerts using the SIM800L GSM Module**.

It is built for:
- Smart firefighting automation.
- Real-time fire & gas detection in industrial/home environments.
- Emergency alerts via SMS even when no internet is available.

---

## 🎯 Features
- 🔥 Fire Detection using IR Flame Sensors
- 🧪 Gas Leakage Detection via MQ2 Sensor
- 🎥 Real-Time Camera Monitoring
- 📲 GSM-based SMS Alerts using SIM800L
- 🔔 Buzzer & LED alerts on fire/gas detection
- 🧭 Manual or Autonomous Navigation Mode
- 🔋 Powered via battery + on-board power module


## 🛠️ Tech Stack & Components Used

### ⚙️ Hardware:
| Component              | Description                                     |
|------------------------|-------------------------------------------------|
| Arduino UNO            | Main microcontroller                            |
| Flame Sensors (2x)     | Detect fire or flame within range               |
| MQ2 Gas Sensor         | Detects combustible gas leakage                 |
| SIM800L GSM Module     | Sends SMS to predefined emergency contacts      |
| Camera Module          | For real-time fire area visuals                 |
| Buzzer + LED           | Local alert system                              |
| Motor Driver (L298N)   | For movement of robot                           |
| Chassis + Wheels       | Mechanical base                                 |
| 18650 Battery + Holder | Power supply                                    |

### 🖥️ Software:
- Arduino IDE
- Embedded C/C++
- PlatformIO (optional)
- PuTTY or Serial Monitor
- GSM AT Commands

---

## 🧠 Working Principle

1. **Sensing Layer:**
   - Flame sensors detect fire visually.
   - MQ2 sensor detects smoke/gas leakage.

2. **Processing:**
   - Arduino UNO reads values from sensors.
   - On threshold detection, alerts are triggered.

3. **Actuation & Alert:**
   - Camera captures live visuals.
   - SIM800L sends SMS with predefined message.
   - Buzzer and LED indicate local alerts.

4. **Mobility:**
   - Robot can be moved manually or navigate autonomously.

---

## 🖼️ Block Diagram

```

\[Sensors]
\|--> Flame Sensor
\|--> MQ2 Gas Sensor
↓
\[Arduino UNO] ---> \[Camera] --> \[Visual Feed]
↓
\[SIM800L GSM] --> \[SMS Alert]
↓
\[Buzzer + LED]
↓
\[L298N Motor Driver] --> \[Wheels]

````

---

## 🧪 Testing & Output

- ✅ Fire tested using matchstick and lighter
- ✅ Gas tested using butane (lighter gas)
- ✅ SMS successfully received within 3 seconds
- ✅ Buzzer and LED alert work in real time
- ✅ Camera provides clear visual data in daylight

---

## ⚠️ Possible Challenges

| Issue | Cause | Solution |
|------|-------|----------|
| SIM800L not responding | Voltage mismatch | Use proper buck converter (3.7–4.2V) |
| No SMS sent | Wrong baud rate or AT command | Double-check serial and use `AT+CMGF=1` |
| False fire detection | Noise/light interference | Calibrate threshold or use IR filters |
| Power drain | SIM800L + Motors draw high current | Use separate battery for GSM module |
| Noisy sensor data | Environmental fluctuations | Add delay or averaging algorithm |

---

## 📷 Project Media

> You can upload pictures/videos in the `assets/` folder and embed them like below.

![Fire Detection Demo](assets/fire-demo.gif)

---

## 📁 Project Structure

```bash
Next-Gen-Fire-Fighting-Robot/
├── code/
│   ├── fire_robot.ino        # Main Arduino code
│   └── AT_commands.txt       # Test AT commands for GSM
├── assets/
│   ├── fire-demo.gif         # Demo media
│   └── wiring-diagram.jpg    # Circuit connection image
├── README.md                 # This file
└── LICENSE
````

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Anirban3030/Next-Gen-Fire-Fighting-Robot.git
cd Next-Gen-Fire-Fighting-Robot
```

### 2. Upload the Arduino Code

* Open `fire_robot.ino` in Arduino IDE
* Select board: `Arduino UNO`
* Select correct COM Port
* Upload code

### 3. Circuit Setup

* Refer to wiring-diagram in `assets/wiring-diagram.jpg`

### 4. Test Fire & Gas Detection

* Use matchstick or gas spray to trigger alert system
* Check SMS received on your phone

---

## 📞 Contact

For queries, feedback or collaboration, feel free to reach out:

**Anirban Paul**
📧 \[[your.email@example.com](mailto:your.email@example.com)]
🔗 [LinkedIn Profile](https://www.linkedin.com/in/your-profile)
🌐 GitHub: [Anirban3030](https://github.com/Anirban3030)

---

## 📝 License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for more information.

```

---

### ✅ Steps to Use It:

1. Go to your GitHub project repo.
2. Click on `Add File > Create new file`.
3. Name the file as `README.md`.
4. Paste the above content and adjust:
   - Your LinkedIn and email.
   - Add actual media files (`fire-demo.gif`, `wiring-diagram.jpg`).
5. Commit the changes.

If you want, I can also create a short **project description** or **LinkedIn post** based on this. Let me know!
```
