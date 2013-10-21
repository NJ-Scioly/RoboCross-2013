RoboCross-2013
==============

Arduino nunchuk controlled car for Science Olympiad RoboCross event 2013

This code was designed to work with continuous servos, esp. Vex 2 wire servos controlled with a Motor controller 29 (an H-Bridge).
A nunchuk is designed to control the servos.

This code was tested on an Arduino Uno.

Circuit:
* Servos:
  * +5V to red wire (external source recommended to reduce jitter, I just cut out a USB wire)
  * Ground to black (if an external source is being used, it's ground should also be connected to the arduino's ground, all the grounds must connect)
  * Pins defined in setup() function, these may be redefined!

* Nunchuk: (reference this pinout: http://voidbot.net/images/pinout-nunchuck-wii-motion-connector.jpg )
  * Analog 5 to Clock (yellow wire)
  * Analog  4 to Data (green wire)
  * +3.3V to power (red wire) (+5V will work, but may lower your controllers lifespan, better safe than sorry)
  * Ground to GND (back wire)

* [Optional] Decoupling Caps
  * Attach various capacitors between +5V and GND and between +3.3V and GND, this will reduce jitter
