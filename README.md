My attempt to a Weather Stetion using ESPHome and Home Assistant.

The main objective is to command the closing of an awning in case of strong wind or rain, but thinking that using ESP32 just to read data from an anemometer was a waste, I added a temperature sensor and a rain bucket.


It is mostly borrowed code from the great work of:
- https://github.com/hugokernel/esphome-weather-station
- https://github.com/hugokernel/esphome-rain-detector
- https://esphome.io/components/sensor/dallas.html
- https://github.com/devjklein/esphome-weatherstation/tree/main


##GPIO used

- GPIO33 rain sensor analog _(see connection diagram [https://github.com/hugokernel/esphome-rain-detector/blob/master/images/circuit_rain_detector.png] )_
- GPIO27 rain sensor power pin 
- GPIO13 anemometer pulse
- GPIO14 rain gauge pulse
- GPIO32 Dallas Temperature _(connect a resistor of about 4.7KΩ between 3.3V and the data pin)_
