# Temperature Data Logger using Arduino Mega

This repository contains the code and documentation for a Temperature Data Logger using Arduino Mega. The project utilizes various components to log temperature data, including DHT11 for temperature and humidity sensing, DS3231 for accurate timekeeping, a Micro SD card for data storage, and an LCD Keypad Shield 16x2 to display live data and time.

## Components Used

- **Arduino Mega:** The main microcontroller responsible for running the data logging code.
- **DHT11:** A sensor used for measuring temperature and humidity.
- **DS3231:** A real-time clock module to provide accurate time and timestamps for the logged data.
- **Micro SD Card:** Used for storing temperature data in a persistent manner.
- **LCD Keypad Shield 16x2:** Display module for showing live data and time, and also for user interface control.

## Functionality

The Arduino Mega runs a program that reads temperature and humidity values from the DHT11 sensor, records the data along with accurate timestamps from the DS3231 module, and stores it on the Micro SD card. Additionally, the live data and time are displayed on the LCD Keypad Shield 16x2. The logged data is also printed to the serial port in a specific pattern, making it accessible for further analysis through different software by manipulating the serial monitor text.

## Getting Started

1. **Hardware Connections:**
   - Connect the DHT11, DS3231, Micro SD Card, and LCD Keypad Shield 16x2 to the Arduino Mega following the provided schematics (https://github.com/vikky0218/Temperature-Data-Logger-Arduino/blob/main/CircuitDiagram.png).

2. **Software Setup:**
   - Install the necessary libraries for DHT11, DS3231, and SD card (provide links to libraries).
   - Upload the Arduino sketch (`Data-Logger_MEGA.ino)`) to your Arduino Mega.

3. **Usage:**
   - Power on the Arduino Mega with the connected components.
   - Open the Serial Monitor in the Arduino IDE or your preferred serial communication software to view the logged data.

## Contributing

Feel free to contribute to the development of this project by opening issues or pull requests. Your feedback and improvements are highly appreciated.

