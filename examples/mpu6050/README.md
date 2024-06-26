# Setup
1. Change network name and password in the ```main.ino``` for you current WiFi network
2. Connect ESP32 with a MPU6050 module using the wiring below:
```
MPU6050:            ESP32:
VCC         →       3.3v
GND         →       GND
SCL         →       D22
SDA         →       D21
```

3. If you haven't already, install the core for ESP32:
 - Open the Arduino IDE.
 - Go to File > Preferences.
 - In the "Additional Board Manager URLs" field, add the following URL: https://dl.espressif.com/dl/package_esp32_index.json
 - Click OK to close the Preferences window.
 - Go to Tools > Board > Boards Manager...
 - Search for "esp32" in the Boards Manager search bar.
 - Install "esp32" by Espressif Systems.
 
 4. Install the libraries for the ESP32 using the build in libraries for Arduino IDE. Install
```
ArduinoJson.h by "Benoît Blanchon"
MPU6050.h by "Electronic Cats"
```
The rest of the libraries are installed automatically by installing the ESP32 core.

5. Upload ```main.ino``` code to ESP32
6. View the serial monitor to see the ESP32 WiFi status (connected or not) and the local IP (i.e. ```192.168.1.39```). Just to double check, you can enter the IP address into a search engine. A string of the JSON data will appear.
7. Update the IP address of the ESP32 in the loggers (view main README for details).