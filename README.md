# ESP8266 Gate Control
Use Esp8266 to control your Electronic Gate

## How (based on my setup)
- A usable remote control for your Electronic Gate
- Relay to control which buttons to fire for your Electronic Gate's remote control
- Brain and hands :D

# Usage
1. Add your wifi credentials & ota credentials in `MySecrets.h` by following the `MySecrets.h.example`
2. Access <your_local_ip_to_esp8266>/1 (HTTP GET) on browser to trigger button 1
3. Access <your_local_ip_to_esp8266>/2 (HTTP GET) on browser to trigger button 2
4. Access <your_local_ip_to_esp8266>/update (HTTP GET) on browser to upload new firmware (`xxx.bin`)
    > use your configured ota credentials (`OTA_USERNAME` & `OTA_PASSWORD`) to access the page

## Library Dependencies
- [esphome-ESPAsyncTCP](https://github.com/mathieucarbou/esphome-ESPAsyncTCP/tree/v2.0.0) - v2.0.0
- [ESPAsyncWebServer](https://github.com/mathieucarbou/ESPAsyncWebServer/tree/v3.3.1) - v3.3.1
- [ElegantOTA](https://github.com/ayushsharma82/ElegantOTA/tree/3.1.5) - v3.1.5