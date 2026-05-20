# LED Blimk Simulation (Arduino - Tinkercad)

## Overview
This project is a simple Arduino UNO LED blink simulation built using Tinkercad.It shows how digital output pin can control an LED using basic timing.

## Purpose
To understand the basic of
- Arduino digital output control
- LED control
- Using delay for timing
- Circuit simulation using Tinkercad

## Component Used
- Arduino UNO R3
- LED (2)
- 220 ohms resistor (2)
- Breadboard
- Jumper wires
- Tinkercad simulatior

## How it works
When the Arduino starts, it sets pin 12 and pin 4 as outputs.
The program then runs in a continuous loop.
First, the LED connected to pin 12 turns ON while the LED on pin 4 turns OFF.
After 1 second, the state changes: the LED on pin 12 turns OFF and the LED on pin 4 turns ON.
This switching continues repeatedly, creating an alternating blinking pattern between both LEDs.

## Code
// C++ code

// Define the pins for easier reading

int ledLeft = 12;

int ledRight = 4;

//

void setup()
{

  //Set both pins as OUTPUT
  
  pinMode(ledLeft, OUTPUT);
  
  pinMode(ledRight, OUTPUT);
        
    
}

void loop()
{

// Turn the left LED on and right LED off

  digitalWrite(ledLeft, HIGH);
  
  // Wait for 1000 millisecond(s)
  
  digitalWrite(ledRight, LOW);
  
  delay(1000);
  
  // Wait for 1000 millisecond(s)
  
// Turn the left LED off and right LED on

  digitalWrite(ledLeft, LOW);
  
  digitalWrite(ledRight, HIGH);
  
  delay(1000);
}
  
## Simulation Link
https://www.tinkercad.com/things/cYIsqlVVaIB-arduino-led-light-blink-demo

## What i learned
- Basic microcontroller output
- Role resistor play in protecting LED light
- How delay contols timing
- Basic circuit simulaation

## NOTE 
This is my first simple embedded system simulation project. I will be improving and building more complex project as i continue learning.

