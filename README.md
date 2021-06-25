# HamsterWheel
Since a few weeks we have a hamster. Her name is Elise.
<insert cute photo of Elise>

Elise likes running in her hamsterwheel and the question keeps on my mind everyday how much did she run?
In order to record her runs there is some hardware involved. For this is also a good oppurtunity to teach myself
a bit about MQTT, Node-Red, Graphana and programming in C++(ESP8266 / ESP32) with PlatformIO.

There are many, many examples on the internet but, the nice ones(well implemented) didn't bother to share the code.
They show nice graphs and explain the journey to the end product but don't mention the important stuff.
Or I can't copy paste it and use it for my own purpose. Also this doesn't help me to get aquainted with the subjects mentioned.
So for this journey I'm going to built everything myself. Well explained so others are able to use it as well.

After giving it some thought on how to track the rotations on the wheel I came up with the following options:
- Add a marker on the outside of the wheel, take turns with my girlfriend and count the rotations by hand
	Then calculate the traveled distance, put them in an Excel sheet and make a nice graph out of it.......
- Glue a small stick on the wheel and count the rotations with an infrared sensor
- Glue a small stick on the wheel and count the rotations with an vibration sensor
- The use of some magnets and a reedswitch
- The use 1 magnet and 2 hall sensors
- Other solutions, like attaching a wheel and count the rotations or others

I'm going for the solution with 2 hall sensors and 1 magnet.
Using this setup I'm able to track in which direction she likes to run and determine when she is just running or secretly try
to fool the measurements by triggering the sensor and quickly walk back and forth while the wheel doesnt turn but the sensors keeps
on triggering.

## Hardware
For measuring I'm using the following:
- Wemos D1 / Wemos D1 32
- 2 hall sensor
- 1 neodium magnet

## Dashboard
- Raspberry Pi
- Docker
- Docker: Mosquitto(MQTT), Node-Red, Graphana

More specifics will follow :)