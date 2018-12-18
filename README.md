# NodeMCUStuff

A collection of stuff I learned while getting the HiLetgo New Version ESP8266 Development board up and running.

See issues for photos for board identification

1. Install the USB to Serial drivers for Win7 or whatever platform you are developing on.
2. It has a built in usb to serial converter so you do not need FTDI or anything to upload from the Arduino IDE to the board
3. Many example sketches say to use "Generic ESP8266 Board" this prevented me from uploading to the board, sorry do have the error, but it was some sort can not write error. When I selected the more specific board I had things worked fine, "NodeMCU 1.0 (ESP-12E Module)"
4. I used the alternative "DHT sensor library for ESPx" instead of the standard DHT library as it is supposed to solve timing issues specific to the ESP boards.
5. The DHT library I used required the GPIO pin number, not the D4 pin identifier on the board. 
