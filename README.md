Smart Temperature Monitor — IoT & Embedded Systems Project

A simple embedded systems mini-project simulating a **Smart Temperature Monitor** using an Arduino UNO and a DHT22 sensor. The system continuously reads temperature and humidity, displays status via LEDs, and triggers a buzzer alert when the temperature crosses a defined threshold.

 Built as part of Project Task-1: Introduction to Embedded Systems & IoT Device Design



 Overview
Embedded systems combine hardware and software to perform dedicated real-time tasks. This project demonstrates a basic IoT-style embedded application: a temperature monitoring and alert system, simulated on **Wokwi** (or buildable on real Arduino hardware).

 Features
- Real-time temperature & humidity readings from a DHT22 sensor
- Visual status via Green (normal) / Red (alert) LEDs
- Audible buzzer alert when threshold is crossed
- Step-by-step Serial Monitor logging for easy debugging/demo

 Hardware / Simulation Components
 Component | Purpose 

|Arduino UNO , Microcontroller 
| DHT22 Sensor , Temperature & humidity sensing 
| Green LED | Indicates normal temperature |
| Red LED | Indicates alert/overheating |
| Buzzer | Audible alert |
| 220Ω Resistors (x2) | Current limiting for LEDs |

 Circuit Diagram
| Component | Arduino Pin |

| DHT22 Data | Pin 2 |
| DHT22 VCC | 5V |
| DHT22 GND | GND |
| Green LED (+) | Pin 8 |
| Red LED (+) | Pin 9 |
| Buzzer (+) | Pin 10 |



How It Works

1. The DHT22 sensor reads temperature and humidity every 2 seconds.
2. If temperature exceeds the threshold (default: **30°C**):
   - Red LED turns ON
   - Buzzer turns ON
   - Green LED turns OFF
3. If temperature is within normal range:
   - Green LED turns ON
   - Red LED and buzzer stay OFF
4. All readings and system states are logged to the Serial Monitor.




PROJECT (WOKWI)

https://wokwi.com/projects/469773961856659457
