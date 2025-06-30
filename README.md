# HOME-AUTOMATION-SYSTEMS

COMPANY : CODTECH IT SOLUTIONS

NAME : KOMPELLA KIRANMAYI

INTERN ID : CTO4DF1700

DOMAIN : INTERNET OF THINGS

DURATION : 4 WEEKS

MENTOR : NELLA SANTOSH KUMAR

DESCRIPTION:
Home automation is the use of technology to control appliances and systems automatically. This project demonstrates a basic home automation system using Arduino UNO, where home appliances (represented by LEDs) are controlled based on the ambient light intensity measured by a photoresistor (LDR - Light Dependent Resistor). The system mimics a smart lighting setup that can turn lights ON or OFF based on surrounding brightness.

Components Used Arduino UNO
A microcontroller board based on the ATmega328P, used to read sensor inputs and control output devices like LEDs.
Breadboard
A platform for building and testing electronic circuits without soldering.
LEDs (Light Emitting Diodes) – Red and Yellow
Act as indicators representing the appliances being controlled.
LDR (Light Dependent Resistor)
A light sensor whose resistance decreases with increasing incident light intensity.
10kΩ Resistor
Used in a voltage divider circuit with the LDR to convert light intensity to a measurable voltage for the Arduino.
220Ω Resistors (x2)
Current limiting resistors for the LEDs to prevent burning them out.
Jumper Wires
To connect all components on the breadboard and Arduino.
USB Cable
Used to power the Arduino and upload code from the computer.

Software Used Arduino IDE (Integrated Development Environment)
Used to write, compile, and upload the code to the Arduino board. Available for Windows, macOS, and Linux.
Tinkercad Circuits (Optional – for Simulation)
A web-based simulator by Autodesk used to simulate Arduino circuits online before physical implementation.

Circuit Connections LDR Sensor Connection:
One leg of the LDR is connected to the 5V supply on the Arduino.
The other leg is connected to the A0 analog pin of Arduino and also to one leg of a 10kΩ resistor.
The other leg of the 10kΩ resistor is connected to GND.
This forms a voltage divider circuit that gives a varying voltage at A0 based on light levels.
Red LED Connection:
The anode (long leg) of the red LED is connected to digital pin 2 on Arduino through a 220Ω resistor.
The cathode (short leg) is connected to the GND rail on the breadboard.
Yellow LED Connection:
The anode is connected to digital pin 3 via another 220Ω resistor.
The cathode goes to GND.
Power Connections:
The 5V and GND pins on Arduino are connected to the breadboard's power rails for common power distribution.
Working of the System The LDR measures the light intensity of the surroundings. The voltage at A0 changes depending on how bright or dark the environment is.
The Arduino reads the analog value using the analogRead() function.
Based on a threshold value (e.g., 500), the Arduino decides whether to turn on or off the LEDs.
If it’s dark (low light):
Analog value from LDR is high → Arduino turns ON the LEDs (as if switching on home lights).
If it’s bright (daylight):
Analog value is low → LEDs are turned OFF.
This creates an automatic lighting system for home automation that saves energy.
output of picture :

