# IoT Real-time Fire Detection Project

## Overview

The IoT Real-time Fire Detection System is a comprehensive Internet of Things solution designed for automated fire detection and environmental monitoring. This system integrates ESP32-based sensor networks with a Flask web application to provide continuous monitoring, real-time data visualization, and immediate alert notifications for fire detection scenarios.

## Features

-   **User Authentication**: Secure login system to manage user access.
    
-   **Real-Time Monitoring**: Display of sensor data and device statuses.
    
-   **Device Control**: Interface to send commands to IoT devices.
    
-   **Responsive Design**: Optimized for various screen sizes and devices.
    
-   **Arduino Integration**: Sensor data collection and transmission using ESP32-based microcontrollers.
    

## Hardware Components

The project utilizes the following Arduino-compatible hardware:

-   2x **ESP32 Devkit V1** boards (Wi-Fi enabled microcontrollers)
    
-   2x **ESP32 GPIO Expanders** for additional input/output pins
    
-   4x **MQ4 Gas Sensors** for detecting methane and other gases
    
-   4x **DS18B20 Temperature Sensors** for precise temperature readings
    
-   4x **Flame Sensors** to detect fire or high-heat sources
    
-   Jumper wires for circuit connections
    

### Arduino Functionality

-   The ESP32 boards collect sensor data (gas, temperature, flame), transmit it to Firebase cloud and the Flask backend collect the data.
    
-   Each `.ino` file (Arduino sketch) defines logic for initializing sensors, connecting to Wi-Fi, and sending data.
    
-   Example sketches:
    
    -   `1st-ESP32.ino`: Manages sensor input and sends data to Firebase.
        
    -   `2nd-ESP32.ino`: Secondary board support sensor expansion.
        

## Technologies Used

### Programming Languages

-   **HTML (61.3%)**: Structure of web pages.
    
-   **CSS (22.8%)**: Styling and layout.
    
-   **SCSS (9.7%)**: Enhanced CSS with variables and nesting.
    
-   **Python (5.6%)**: Backend logic and server-side operations.
    
-   **JavaScript (0.6%)**: Client-side interactivity.

-   **C++**: Hardware components.

### Frameworks and Libraries

-   **Flask**: Lightweight Python web framework for backend development.
    
-   **Jinja2**: Templating engine used with Flask for dynamic HTML rendering.
    
-   **Bootstrap**: CSS framework for responsive design.
    

### Development Tools

-   **IDEs**: Visual Studio Code, Arduino
    
-   **Version Control**: Git, GitHub
    
### Cloud Service

-   **Firebase**: Capture data from the microcontrollers and let the web backend get those data.

```
IOT Real-time Fire Detection system/
├── app.py
├── requirements.txt
├── templates/
├── static/
├── users.txt
├── alarm.mp3
├── README.md
└── Arduino/
    ├── 1st-ESP32.ino
    └── 2nd-ESP32.ino

```

-   `app.py`: Main Flask application file.
    
-   `templates/`: HTML templates rendered by Flask.
    
-   `static/`: CSS, JS, and static assets.
    
-   `users.txt`: Stores user credentials.
    
-   `alarm.mp3`: Audio alert file.
    
-   `Arduino/`: Contains Arduino sketches for ESP32 devices.
    


