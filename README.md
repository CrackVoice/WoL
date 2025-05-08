# BASED ON ORIGINAL WORK BY [LUCKERIS](https://github.com/Luckeris)
# ESP32 PC Control with Wake-on-LAN (Python & C++ Versions)

This project allows you to control your PC via Wake-on-LAN (WOL) technology using the ESP32. It includes both **Python** and **C++** implementations. Using a simple web interface, you can power on your PC or restart the ESP32 device.

The code is a rewrite of the original C++ version by [Luckeris](https://github.com/Luckeris) with a Python alternative added for flexibility and learning purposes.

## Features
- Web interface for PC control
- Wake-on-LAN functionality
- ESP32 restart option
- Written in both Python (MicroPython) and C++ (Arduino)

## Requirements
- ESP32 board (e.g., ESP32 Dev Kit)
- WiFi network
- A PC with Wake-on-LAN enabled
- Arduino IDE (for C++ version)
- Thonny or similar (for MicroPython version)

## How to Use

1. **Configure Network Settings**:
   Set your specific parameters in the code:
   - `ssid`: Your WiFi network name
   - `password`: Your WiFi password
   - `macAddress`: MAC address of the PC you want to wake
   - `pcIP`: IP address of the target PC

2. **Upload to ESP32**:
   - **C++**:
     - Open the C++ version in Arduino IDE
     - Select the correct ESP32 board and COM port
     - Upload the sketch
   - **Python**:
     - Flash MicroPython to the ESP32
     - Upload the Python script using Thonny or ampy

3. **Access the Web Interface**:
   - Monitor the serial output to find the ESP32’s IP address
   - Enter the IP address in your browser on the same WiFi network

4. **Control PC**:
   - **Turn On PC**: Sends the WOL magic packet
   - **Restart ESP32**: Reboots the ESP32

## Credits
Original project by [Luckeris](https://github.com/Luckeris).  
Python and additional improvements by [CrackVoice](https://github.com/CrackVoice).

## License
This project is open-source and available under the MIT License.
