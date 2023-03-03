# ESP32_OTA_APMODE
This is a sample code for using OTA on Access point mode.  Previously an issue happened on AP or offline connections where the ESP32 tried to import jquery.min.js from Google API. Obviously, this doesn't work, as there is no internet. To fix this, we can either embed the file on SPIFFS, or convert it to binary and just paste on our code.    

This will increase the program size by ~30 kb,  instead of ~140kb from the original file + spiffs lib.  No additional libraries needed.  Works fine on PlatformIO.

reference 1: https://randomnerdtutorials.com/esp32-over-the-air-ota-programming/
reference 2: https://esp32.com/viewtopic.php?t=11744
