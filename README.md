mostly borrowed code from the great work of:
- https://github.com/hugokernel/esphome-weather-station
- https://github.com/hugokernel/esphome-rain-detector
- https://esphome.io/components/sensor/dallas.html


##GPIO

- GPIO33 rain sensor analog _(see connection diagram [https://github.com/hugokernel/esphome-rain-detector/blob/master/images/circuit_rain_detector.png] )_
- GPIO27 rain sensor power pin 
- GPIO13 anemometer pulse
- GPIO14 rain gauge pulse
- GPIO32 Dallas Temperature _(connect a resistor of about 4.7KΩ between 3.3V and the data pin)_
