# esp32-weatherstation
ESP32 based temperature and humidity sensor with Web config support 

Allows users of ESP32 boards to configure in which WLAN the board should connect to. By pressing the ESP32 board 'boot' button 
the board is set to configuration mode and opens a WLAN access point with SSID 'SETUP' and IP 192.168.4.1.
You can then access the board by using your webbrowser and enter the WLAN network ssid and password which are then stored into
the ESP32 boards persistant EEPROM. 
Then the board has all the necessary info to boot and connect into your configured WLAN as a client device. 

The config process is repeated when the ESP32 board is unable to connect to your WLAN or when you press the 'boot' button again.
