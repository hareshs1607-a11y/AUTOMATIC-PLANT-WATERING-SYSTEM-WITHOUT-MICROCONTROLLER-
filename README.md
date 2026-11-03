Watering plants regularly is one of the most common problems in plant care, especially when the owner is away from home for several days.
Over-watering damages the roots, while under-watering dries the plant. Most automatic watering solutions use a microcontroller such as an Arduino, which adds cost, wiring and programming effort.
This project presents an Automatic Plant Watering System that is built entirely from basic analog components and does not need any microcontroller or program code.
A soil moisture sensor continuously monitors the soil. Its output controls a chain of three BC547 NPN transistors, which switch a small 5 V DC water pump.
The first transistor (Q1) discharges a timing capacitor whenever the soil is dry. The second transistor (Q2) works as an inverter, and the third transistor (Q3) drives the pump. 
A resistor–capacitor (RC) timer, made of a 100 kΩ potentiometer and a 680 µF electrolytic capacitor, keeps the pump running for an adjustable time after the soil becomes wet, so that the soil is watered properly and the pump does not switch ON and OFF rapidly. 
A 1N4007 diode connected across the pump protects the driver transistor from the voltage spike produced when the motor is switched off.
The circuit was designed using standard component values, verified by calculation, simulated in TinkerCAD and assembled on a breadboard with a potted plant, a water bottle and a mini submersible pump.
It works from a single 5 V supply, the watering time can be adjusted with the potentiometer, and the whole circuit costs only a few hundred rupees.
This report describes the theory of each part of the circuit, the design calculations, the step-by-step implementation and testing procedure, the results, the limitations and the possible improvements of the system.
Keywords: Soil moisture sensor, BC547 transistor, RC timer, inverter, flyback diode, water pump, automatic irrigation.
