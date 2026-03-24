# Embedded Heart Rate & HRV Monitoring System

## Overview
This project is an embedded system designed for measuring heart rate and heart rate variability (HRV) in real time. The system processes sensor data locally, stores historical measurements, and transmits data to cloud services for further analysis.

## Key Features
- Real-time heart rate and HRV monitoring  
- Signal processing with real-time filtering for accurate data  
- MQTT-based communication with cloud services  
- Wi-Fi connectivity for cloud communication and time synchronization (NTP)  
- Local data storage for historical tracking and analysis  
- Real-time data visualization on Raspberry Pi OLED display  

## My Contributions
- Led system design and development, defining architecture and distributing tasks across the team  
- Applied real-time signal filtering for accurate sensor data processing  
- Designed and implemented local data storage for historical analysis  
- Streamed sensor data to cloud services using MQTT  
- Developed real-time visualization on Raspberry Pi OLED display using MicroPython  

## Technologies
- MicroPython    
- Raspberry Pi
- Wi-Fi
- NTP
- MQTT  
- Kubios Cloud  

## System Architecture
The system consists of:
- Sensor data acquisition  
- Local signal processing (filtering)  
- Wi-Fi connectivity via router  
- Data transmission via MQTT  
- Time synchronization using NTP  
- Cloud-based analysis  
- Local visualization on OLED display   

## Key Implementation
Main components of the system:
- Signal processing: `/src/hrlib.py`  
- MQTT communication: `/src/mqtt.py`
- Kubios Cloud: `/src/kubios.py`  
- Data storage: `/src/history.py`  

## How It Works
1. Device connects to a Wi-Fi network via router  
2. System synchronizes time using NTP after successful Wi-Fi connectivity
3. Sensor data is collected from the heart rate sensor  
4. Data is filtered in real time to remove noise    
5. Processed data is given an NTP timestamp and stored locally for later use.
6. User chooses data to be sent to Kubios Cloud via MQTT.  
7. Results are visualized on an OLED display   

## Team
Developed as part of a team project.

## Future Improvements
- Enhanced data visualization dashboard  
- Improved signal processing algorithms  
- Mobile or web-based interface for monitoring
- Communication between each team member

## Author
Souci Sami
