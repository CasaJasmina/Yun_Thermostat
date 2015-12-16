# Yun_Thermostat
####Controlling home's thermostat with Arduino Yun
The Yun_Thermostat is a really simple temperature sensor connected to a relay, which close the contact when temperature goes under a certain threshold. It can be attached to the boiler so that it can swich on and off automatically.

<img src="https://github.com/CasaJasmina/Yun_Thermostat/blob/master/Img/Yun_thermostat.jpg" width="400" /> 

##Connecting wires
<img src="https://github.com/CasaJasmina/Yun_Thermostat/blob/master/Img/Fritzing_sketch.png " width="400" /> 

##Loading sketches
[Here](https://github.com/CasaJasmina/Yun_Thermostat/tree/master/Thermostat-relay) you can find a really basic Arduino sketch ready to be loaded.</br>
In order to read values from the sensor you have to import the [library](https://github.com/adafruit/DHT-sensor-library).

##Notes about the sensor
<img src="http://www.electroschematics.com/wp-content/uploads/2015/02/DHT22-PinOut.png" width="200" /></br>
The DHT22 sensor, used in this project, has a really simple [datasheet](https://www.sparkfun.com/datasheets/Sensors/Temperature/DHT22.pdf):</br>
Pin one has to be plugged in the 5V and is used for power supply</br>
Pin two is for data and it can be plugged in every pin depending on your needs</br>
Pin three unused</br>
Pin four has to be plugged in the ground

##Notes about the ralay
<img src="https://github.com/CasaJasmina/Yun_Thermostat/blob/master/Img/Relay.png " width="200" /> </br>
The A1 and A2 pins provide current needed to operate, connect one to the ground and the other one to the 5V.
Others pins are symmetric, so you can use only one side.</br>
Connect 21 and 24 (or 11 and 14) for a normally closed connection.</br>
Connect 22 and 24 (or 12 and 14) for a normally open connection.

[Here](http://datasheet.octopart.com/30.22.7.005.0010-Finder-datasheet-22148898.pdf) the datasheet.

###BOM

| part		        | Quantity | Type | LINK|
| -------------     |:--------:| :--------:| :--------:|
| Arduino Yun       | 1 |  | https://www.arduino.cc/en/Main/ArduinoBoardYun| 
| Proto shield      | 1 |  | https://www.arduino.cc/en/Main/ArduinoProtoShield |
| Relay             | 1 | 2A signal relay	|  |
| Transistor        | 1 | BC54 |  |
| 10k resistor      | 2 |  |  |
| 220 resistor      | 1 |  |  |
| Led               | 1 | 	|  |
| Screw terminal    | 1 |  |
| Diode             | 1 | 1n4001	|  |

####Credits

Project developed by Tommaso Laterza for [Casa Jasmina](http://casajasmina.arduino.cc/).
