# Temperature Data Logger using Arduino Mega

This repository hosts the code and schematics for a robust temperature and humidity data logger built using Arduino Mega. The system reads environmental data, logs it with timestamps, displays real-time readings, and provides future-proof functionality for data analysis.

## Table of Contents
1. [Features](#features)
2. [Components Used](#components-used)
3. [Schematics](#schematics)
4. [Setup Instructions](#setup-instructions)
5. [Serial Communication Format](#serial-communication-format)
6. [Contributing](#contributing)
7. [License](#license)

## Features
- **Real-Time Data Logging:** Logs temperature and humidity with precise timestamps.
- **Data Storage:** Saves readings in CSV format on an SD card for long-term storage.
- **Live Data Display:** Shows current temperature, humidity, and time on a 16x2 LCD screen.
- **Persistent Configuration:** Ensures last configuration settings are retained using SD card storage.
- **Serial Output:** Provides logged data in a structured format for software integration.

## Components Used
- **Arduino Mega:** Controls the system.
- **DHT11 Sensor:** Measures temperature and humidity.
- **DS3231 RTC Module:** Supplies accurate time for timestamps.
- **Micro SD Card Module:** Stores logged data persistently.
- **LCD Keypad Shield 16x2:** Displays live data and provides user interface control.
- **Breadboard & Jumper Wires:** For prototyping and connections.

## Schematics
Refer to the provided circuit diagram:  
[![Circuit Diagram](https://github.com/vikky0218/Temperature-Data-Logger-Arduino/blob/main/CircuitDiagram.png)](https://github.com/vikky0218/Temperature-Data-Logger-Arduino/blob/main/CircuitDiagram.png)

## Setup Instructions

1. **Hardware Connections:**  
   - Assemble the DHT11, DS3231, SD Card module, and LCD Keypad Shield as per the schematics.

2. **Software Prerequisites:**  
   - Install these libraries in Arduino IDE:
     - [DHT Library](https://github.com/adafruit/DHT-sensor-library)
     - [RTCLib](https://github.com/adafruit/RTClib)
     - [SD Library](https://www.arduino.cc/en/Reference/SD)

3. **Upload the Code:**  
   - Open `Data-Logger_MEGA.ino` and upload it to the Arduino Mega.

4. **Viewing the Data:**  
   - Insert an SD card into the module.
   - Open the Arduino Serial Monitor at `9600 baud` to view real-time data and log entries.

## Serial Communication Format
The serial output is structured for easy parsing:
Temperature (°C); Humidity (%); Time (HH:MM:SS); Date (DD/MM/YYYY)

## Contributing
Pull requests are welcome. For major changes, please open an issue to discuss what you would like to modify.

## License
This project is licensed under the [MIT License](LICENSE).
