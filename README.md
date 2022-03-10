# ESP32_OTA_APMODE
This is a sample code for using OTA on Access point mode.  Previusly a issue happened on AP or offline connections where the ESP32 tried to import jquery.min.js from google API.
Obviously this dont work, at there is no internet.  To fix this we can either embed the file on SPIFFS, or convert it to binary and just paste on our code.    

This will increase the program size by ~30KB,  instead of ~140kb from the original file + spiffs lib.  No additional libraries needed.  Works fine on platformio.

Source code: https://randomnerdtutorials.com/esp32-over-the-air-ota-programming/
fix: https://esp32.com/viewtopic.php?t=11744
