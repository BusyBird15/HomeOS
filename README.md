# Introduction and Notes
A simple operating system for the Arduino Uno and Arduino-Uno-compatible boards with a LCD keypad sheild.

* The code is maintained by me.
* The code is registered under The Unliscence.<br><br>

# Materials and Connections

### Modules and Sensors
* **Required:** The DS1302 RTC module. Compatibility for others coming later.
* **Optional:** A DHTxx module, either the DHT11, DHT21, or DHT22 will work.
* **Optional:** Any human IR motion sensor, of where it is `LOW` when motion is detected.
* **Optional:** A photoresistor for detecting ambient light and turning off the backlight at a certain threshold value.
* **Optional:** A 4-ohm speaker, 8-ohm speaker, of piezzoic buzzer. Obviously, this is required for the alarm feature.

### Connections
* The RTC module can connect to any three digital pins. 
* DHT sensor can connect to any digital pin (you may need a 10k pullup resistor).
* Human IR sensor can simply connect to any digital or analog pin.
* A photoresistor can be connected to any analog pin, with a 10k pullup resistor.
* The speaker can connect to any digital pin.<br><br>

# Uploading Code
1. Download the latest release from the right of this page.
2. Download and install the Arduino IDE of your choice from https://arduino.cc.
3. Double-click the code file you just downloaded. Arduino IDE will open, and it may mention that the sketch needs to be in a folder. Click "yes" or "Create folder and open".
4. Connect all your sensors to the Arduino an plug it in. From the Tools menu in the IDE, select your proper board and port.
5. In the first lines of the code you will see an intro and some commented variables. Follow the instructions and modify the variables to your hardware.
6. Click the right arrow (or ctrl+U (cmd+U on mac)) to upload the code.
7. When it finishes, scroll down to the `void setup()` function. You will see a few special commented lines. Comment out the line inside the comment box, then repeat step 6. This automatically calibrates your clock module to the accurate time and date.
