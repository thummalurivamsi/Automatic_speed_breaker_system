# 🚗 Automatic Smart Speed Breaker System Based on Vehicle Speed with IoT

This project presents a smart and innovative solution to prevent overspeeding by dynamically controlling a speed breaker based on the detected vehicle speed. Designed with embedded systems and IoT integration, this project helps improve road safety in sensitive or accident-prone areas.

---

## 📌 Project Overview

Conventional speed breakers often cause discomfort and are not always effective. This system uses **IR sensors** to detect the speed of approaching vehicles. If a vehicle is found overspeeding (exceeding a threshold like 40 km/h), the system triggers a **servo motor** to raise a speed breaker mechanism and alerts nearby entities using a **buzzer and LED**. Data is logged to the cloud using an **ESP8266 Wi-Fi module**, enabling real-time monitoring and analysis.

---

## ⚙️ Components Used

- **Arduino Uno**
- **IR Sensors (x2)** – For speed calculation
- **16x2 LCD** – To display vehicle speed and status
- **Servo Motor** – To simulate the raising/lowering of the speed breaker
- **Buzzer** – Warning alert for overspeeding
- **LEDs (Red & Green)** – Indicate safe or overspeed
- **ESP8266 Wi-Fi Module** – Sends data to the cloud (ThingSpeak or Firebase)
- **Power Supply, Resistors, Connecting Wires**

---

## 🧠 Working Principle

1. Two IR sensors are placed at a fixed distance.
2. As a vehicle crosses the first and then the second IR sensor, the Arduino calculates the time interval to compute speed.
3. If the speed exceeds the defined threshold:
   - The servo motor activates to raise the speed breaker.
   - A buzzer sounds and the red LED turns on.
   - Speed and event data is pushed to the cloud.
4. If the speed is within the limit:
   - The road remains flat.
   - Green LED is turned on.
   - Speed data is still logged.

---

## 🌐 IoT Integration

The **ESP8266 Wi-Fi module** is used to send data (speed, status, timestamp) to a cloud server such as:
- **ThingSpeak** – for real-time data visualization
- **Firebase** – for logging and alerts

This helps in maintaining records of overspeeding and can support authorities in traffic regulation enforcement.

---

## 💡 Features

- Automatic speed detection
- Real-time alerting with buzzer and LEDs
- Cloud integration for remote data monitoring
- Enhances road safety without causing driver inconvenience
- Easy to implement and cost-effective

---

## 📸 Project Media

[Link to Circuit Diagram and Code](https://drive.google.com/file/d/1nGDs6Pp2ZHf9SxvlADdeTeOrwtgM-tXF/view?usp=sharing)

*(You can add actual images/videos in this section once uploaded to GitHub or external hosting.)*

---

## 📈 Future Improvements

- Integration with automatic number plate recognition (ANPR) for logging violators
- Solar power support
- GSM/SMS alert to traffic authorities
- Mobile application interface for live monitoring

---

## 👨‍💻 Developed By

[Your Name]  
[Your Institution or Organization]  
[Email / LinkedIn / Portfolio links, if you'd like]

---

## 🛠️ License

This project is licensed under the MIT License - feel free to use and modify as needed.

