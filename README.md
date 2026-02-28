README.md
# Automatic Streetlight  simulation  control system

## PROJECT VIEW 
The Automatic Street light Control system is designed to automatically switch street lights ON and OFF based on enviromental light intensity. The system uses a light dependent Resistor to dectect daylight and darkness. it helps to reduce enerfy wate and elinimate manual swicthing 

## AIM
To design and implenment an automatic street lighting system the operates based on surrounding light conditions.

## COMPONENT IN TINKERCAD 
Arduino nano
light dependent resistor (LDR)
10kilo ohm's Resistor 
Led
Breadboard 
jumperwires 
powersupply

## COMPONENT IN PROTEUS 
3WATT 10k
3005P-1-102
3009P-1-1003lf
ARDUNIO NANO V£ COMPLETE
BC547BP
LAMP
LM016L
MINRES10K
POT-HG
VSOURCE


## work principles
The system works using the resistance property of the The LDR:
During the day the light intensity is high  LDR resistance is low light remains OFF 
During the night the light intensity is low LDR resistance is high light reamins ON 

The Arduino reads the voltage from the LDR and controls the relay accordingly.


## circuit Description 
The LDR and resistor from a voltage divider circuit connected to the analog input of the Arduino. The relay module is connected to a digtal output pin to control the street light.

## Arduino Code

// pin assigment  

int redLED =9;

int yellowLED=10;

intgreenLED=11;



void setup() { 

// set all LED pins as OUTPut 

 pinmode (redLED, OUTPUT);
 
 pinmode (yellowLED, OUTPUT);
 
 pinmode (greenLED, OUTPUT);
}



 void loop()
 {
 // RED LIGHT ON 
 
digitalWrite(redLED, HIGH);

digitalWrite(yellowLED, LOW);

digitalWrite(greenLED, LOW);

delay(6000); // red stays for 10 seconds



// YELLOW LIGHT ON 

digitalWrite(redLED, LOW);

digitalWrite(yellowLED, HIGH);

digitalWrite(greenLED, LOW);

delay(6000); // red stays for 10 seconds




// GREEN LIGHT ON 

digitalWrite(redLED, LOW);

digitalWrite(yellowLED, LOW);

digitalWrite(greenLED, HIGH);

delay(6000); // red stays for 10 seconds
}



## RESULTS 

the system was successfully turned ON the light during delay .
the light automatically turned OFF during bright conditions. 
the project achieved energy-saving functionally .






