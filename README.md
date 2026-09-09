# CERES.OS
Small operating system for diy smartwaches based on esp32c3 and others

CERES_OS is a custom-built, ultra-lightweight operating system tailored for ESP32-C3 smartwatches equipped with an OLED display. Built around a clean, multi-card user interface, CERES_OS delivers essential wearable functionality with minimal overhead.  

# Key Features:
 - Card-Based UI Navigation: Seamlessly cycle between the Home Screen, Watch Tools (Alarm, Countdown Timer, Stopwatch), Weather Dashboard, and System Status.
 - Automatic Time & Weather Sync: Fetches real-time time via NTP and accurate local weather metrics using non-blocking HTTP requests.
 - Power Management: Integrated ESP32 deep sleep support with quick wake-up handling and dynamic display time-outs.
 - Wi-Fi Manager: Easy setup portal for connecting to local Wi-Fi networks without hardcoding credentials.
 
# Hardware Support: 
Built-in drivers for Adafruit SH1106 OLED displays, WS2812 RGB LEDs, active buzzers, and analog battery monitoring. 

 # Technical Notes & Hardware Required Hardware: 

ESP32-C3 microcontroller, 128x64 I2C OLED display (SH1106G), Active Buzzer, and standard push buttons.  

Core Libraries Required: Adafruit_SH110X, Adafruit_GFX, WiFiManager, ArduinoJson, Adafruit_NeoPixel, and LittleFS.  

# Configuration and instalation: 
Before flashing, set your default location coordinates (String latitude = "**.****"; String longitude = "**.****";) at the top of the main code file to fetch accurate weather data for your region.  
Using Arduino IDE, change dev board options in tools to ones showed on image:
<img width="360" height="315" alt="image" src="https://github.com/user-attachments/assets/f0e6edce-783b-4d21-9a0a-b784f35e2b11" />
