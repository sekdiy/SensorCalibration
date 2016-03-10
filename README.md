# SensorCalibration Library [![Version](https://img.shields.io/badge/SensorCalibration-0.0.1-blue.svg 'still in alpha')](https://github.com/sekdiy/SensorCalibration)

## Proposal:

I'd like to contribute an Arduino/AVR library that makes [calibrating](https://www.arduino.cc/en/Tutorial/Calibration) sensor input a breeze.

It shall be easy to apply, have a simple enough approach which shall still be sufficient for most users, with a small footprint and good Arduino/AVR compatibility.

## Motivation:

My own IoT applications increasingly depend on sensor accuracy and repeatability. I've just recently started the fifth special purpose library where I apply the same calibration/compensation approach again – just to a different sensor.

So I've started writing a library for myself. But during my research I realized that this task seems to be a very generic problem and most people just appear to come up with the same kind of solution over and over again.

The world shouldn't have to be like that! Everyone should be able to take compensated measurements!

## Ideas so far:

 - at least linear two-point compensation (i.e. as [described by Atmel](http://www.atmel.com/images/doc8108.pdf) for the internal temperature sensor)
 - automated [mapping](https://www.arduino.cc/en/Reference/Map) to [min and max](https://en.wikipedia.org/wiki/Normalization_(statistics) values
 - automatic [gain control](https://en.wikipedia.org/wiki/Automatic_gain_control) and [limiting](https://www.arduino.cc/en/Reference/Constrain) of input data
 - support for multiple sensors (portable sensor profiles)

## Question(s):

 - What functionality does an Arduino user expect from a piece of code that claims to support calibrating a sensor?

 - What interface would be appropriate (simple, complex, both)?

 - How much resource consumption would be acceptable, i.e. how lean vs. mighty could the library sensibly become?

 - What prior work has been done regarding universally applicable Arduino/AVR libraries? Is my work futile, have I been bested already?

If you have a question or contribution, please simply open an issue.
