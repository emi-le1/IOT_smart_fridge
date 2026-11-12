# IoT SMART FRIDGE - PROJECT DOCUMENTATION

## 1. Executive Summary
IoT Smart Fridge is an innovative solution that monitors fridge temperature, humidity, door status and food inventory remotely. It helps reduce food waste, save energy, and alert users via mobile phone when fridge conditions are abnormal. Built for Rwandan households and small shops.

## 2. Problem Statement
Many households lose food due to power cuts, leaving fridge door open, or not monitoring temperature. Small shops selling cold drinks/meat lack remote monitoring. Current smart fridges are expensive (>$1000) and not adapted to local context.

## 3. Solution & Features
| Feature | Description | Sensor/Tech |


| Temperature Monitoring | Real-time temp 0-10°C, alert if >8°C | DHT11/DHT22, DS18B20 |
| Door Status | Alert if door open >2 min | Magnetic Reed Switch |
| Remote Access | View data on phone anywhere | ESP32 + WiFi + MQTT |
| Energy Saving | Auto-alert on power loss | Voltage sensor |
| Inventory | Manual entry + expiry reminders | Mobile App |

## 4. System Architecture
**Hardware:** ESP32 Dev Board, DHT22 Temp/Humidity, Magnetic Door Sensor, Buzzer, 5V Relay, Breadboard, 12V Power

**Software:** Arduino C++ firebase+Realtime DB / IoT DataHub, MQTT Protocol

**Mobile:** Android App (MIT App Inventor) or Web Dashboard (HTML/JS/css&react/tailwind css/node.js)

**Data Flow:** Sensors -> ESP32 -> WiFi -> Firebase -> Phone Dashboard -> User Alert

## 5. Prototype Status
Prototype built and tested. Achieves: Temperature reading every 30 sec, Door alert via buzzer + phone notification, Data logged to cloud for 7 days. Next: PCB design, solar backup, Kinyarwanda voice alert.

## 6. Skills Demonstrated
- Embedded C/C++ & Arduino
- IoT Protocols (MQTT, HTTP)
- Hardware wiring & soldering
- firebase/ IoT cloud
- Mobile App basics
- Problem solving & innovation for local needs
