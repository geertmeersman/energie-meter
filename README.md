# Build a cheap water and gas usage sensor using ESPhome, a proximity sensor and a TCRT5000 Infrared Reflective Sensor

In this project I share a walkthrough on how you can build a water and gas usage meter using ESPHome that integrates with your Home Assistant.

## How to read an analog water meter?
I live in Belgium and the water meter I have is a Sensus 520 which has a small spinning wheel with a metal plate.

![Example of a Sensus 520 water meter!](/.resources/sensus-520-water-meter.png "Example of a Sensus 520 water meter")

The solution to read it was by using either a reflective sensor or a proximity sensor.

The implemenation I went for was a proximity sensor [LJ18A3-8-Z/BX-5V]: https://nl.aliexpress.com/item/32826218456.html

![Proximity sensor!](/.resources/proximity-sensor.png "Proximity sensor")

1 spin of the wheel will result in a pulse, every pulse being equal to what has been defined by your meter.

![Proximity sensor on meter!](/.resources/proximity-sensor-on-meter.png "Proximity sensor on the meter")
