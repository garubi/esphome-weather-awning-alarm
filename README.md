My attempt to a Weather Stetion using ESPHome and Home Assistant.

The main objective is to command the closing of an awning in case of strong wind or rain, but thinking that using ESP32 just to read data from an anemometer was a waste, I added a temperature sensor and a rain bucket.

# UPDATE SUMMER 2024
**Apply ideas and code from:**
https://github.com/devjklein/esphome-weatherstation/tree/main
https://community.home-assistant.io/t/measuring-wind-speed/395693/56

The previous installation was messy, unreliable and the data too much confusing.
In this iteration I lost the rain sensor, but since it oxidates very fast, I can't realy on it.

The new version (starting from 2.0) should only be software related. I don't plan to changhe the hardware

**Solar panel powered**
see [Solar readme](Docs/solar_powered_station.MD)


## links
It is mostly borrowed code from the great work of:
- https://github.com/hugokernel/esphome-weather-station
- https://github.com/hugokernel/esphome-rain-detector
- https://esphome.io/components/sensor/dallas.html
- https://github.com/devjklein/esphome-weatherstation/tree/main


## GPIO used

- GPIO33 rain sensor analog _(see connection diagram [https://github.com/hugokernel/esphome-rain-detector/blob/master/images/circuit_rain_detector.png] )_
- GPIO27 rain sensor power pin 
- GPIO13 anemometer pulse
- GPIO14 rain gauge pulse
- GPIO32 Dallas Temperature _(connect a resistor of about 4.7KΩ between 3.3V and the data pin)_
- GPIO34 Battery level
