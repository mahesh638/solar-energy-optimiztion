# solar-energy-optimiztion
This project aims to build a model of a smart solar panel that faces the sun as it moves during the duration of the day. Furthermore, to improve the device by building a Machine Learning model to predict where the panel needs to be facing at different parts of the day to make it usable in any terrain without a sensor. <br/>
<br/>
![solar](/Doc/demo_solar.png)
<br/>
<br/>
The flat platform that the panel is placed in has 4 LDR sensors in the corners. Servo motors are used to rotate the panel. The sensors and the motors are connected to an Arduino Uno which is then connected to a Raspberry Pi. Refer Solar tracking Proj.pptx for more details regarding the circuit <br/>
Firstly, code.uno is run. This code moves the panel according to the direction of the light by observing the light intensity values of the four sensors. Additionally, the sending.py code is run in the Raspberry Pi simultaneously to record the values of the Servo Motor with the timestamp in which it was received. This helps in creating a regression model which will predict the angle in which the Motor needs to turn in different parts of the day. <br/>
<br/>
Finally, the work.py code is run which has the regression model to give values to the servo motor in different times of the day to make it turn towards the sun using this code and not the sensors. </br>

