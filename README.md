# EXPERIMENT-01-INTERFACTING-DIGITAL-OUTPUT-WITH-EDGE-DEVICE---RASPBERRYPI-PICO-
## NAME : S.Dhivyan
## DEPARTMENT : AIDS
## ROLL NO : 21224230067
## DATE OF EXPERIMENT : 24.02.2025

### AIM
To interface a digital output device (LED) with the Raspberry Pi Pico and control it using MicroPython.

APPARATUS REQUIRED
Raspberry Pi Pico
LED (Light Emitting Diode)
330Ω Resistor
Breadboard
Jumper Wires
USB Cable
Computer with Thonny IDE
## THEORY
Raspberry Pi Pico is a microcontroller board based on the RP2040 chip. It supports MicroPython, making it suitable for IoT and embedded applications.

Digital Output refers to controlling external devices like LEDs, buzzers, or relays using GPIO (General Purpose Input Output) pins. A GPIO pin can be set to HIGH (3.3V) or LOW (0V) to turn the device ON or OFF.

## Working Principle:

The LED is connected to one of the GPIO pins of the Pico.
The MicroPython script sets the GPIO pin HIGH to turn the LED ON and LOW to turn it OFF.
CIRCUIT DIAGRAM
Connect the anode (longer leg) of the LED to GP15 via a 330Ω resistor.
Connect the cathode (shorter leg) of the LED to GND (ground).


## PROGRAM (MicroPython)
```
from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
while True:
    led1.toggle()
    sleep(0.5)

    

from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
led2 = Pin(4, Pin.OUT)
led = Pin(10, Pin.OUT)
while True:
    led1.toggle()
    sleep(0.5)
    led2.toggle()
    sleep(0.5)
    led.toggle()
    sleep(0.5)
    


from machine import Pin
from utime import sleep
led1 = Pin(0, Pin.OUT)
led2 = Pin(4, Pin.OUT)
led = Pin(10, Pin.OUT)
buzz=Pin(7,Pin.OUT)
while True:
    led1.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)
    led2.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)
    led.toggle()
    sleep(0.5)
    buzz.toggle()
    sleep(0.5)




 



 


## OUPUT
![Screenshot 2025-02-24 113502](https://github.com/user-attachments/assets/075cbd42-44e2-49c2-849c-065eceb14dcf)

![Screenshot 2025-02-24 113014](https://github.com/user-attachments/assets/b46c17fe-3a4a-4668-9108-6a66c4fc2cbb)
 
![Screenshot 2025-02-24 111646](https://github.com/user-attachments/assets/8693a3c8-7c8c-4b30-9aae-2de744e30a18)



 
## RESULTS
The LED connected to the Raspberry Pi Pico successfully turns ON and OFF at 1-second intervals, confirming the proper interfacing of a digital output.
