# module1lesson1

Component connections and their functions
Connection diagram (based on your school's guide)
Arduino D8 → Resistor → LED Anode (+) → LED Cathode (−) → GND
The resistor is in series with the LED to limit current. The circuit shares a common ground.
Component Connected to Function
Arduino GND Blue (-) rail Provides the ground connection
Arduino Digital Pin 8 One end of 220Ω resistor Supplies the output signal
Other end of resistor A10 Connects the resistor to the LED's positive side
LED Anode (+) E10 Receives current
LED Cathode (-) E11 Returns current toward ground
A11 Blue (-) rail Connects the LED's negative side to ground
How the project works
The Arduino Uno sends an output signal through Digital Pin 8.
The electrical current passes through the 220Ω resistor.
The resistor limits the current to help protect the LED.
The current passes through the LED, making it light up.
The current returns through the ground rail to the Arduino.
Code function
pinMode(8, OUTPUT); – sets Pin 8 as an output.
digitalWrite(8, HIGH); – turns the LED ON.
digitalWrite(8, LOW); – turns the LED OFF.
