<img src="AlarmClock.svg" alt="alarm clock" height="200"/>

# Alarm Clock
An Open-Source, easy to build alarm clock.

## Description
To make sure, that I can be in time I wanted to buy a new alarm clock to have beside my smartphone.  
I wanted one which is reliable, not depending on wall power and I can set, manage multiple alarms easily.  
I searced through some sites, but I could not find any, which I liked.  
So I designed my own.  
I wanted to mimik the clock of a general smartphone and set alarms easily through a touchscreen.  
Because I use an ESP32 I also hope to be able to display some notifications through bluetooth and use other features of it in the future.   

## Hardware
### PCB
It is a nearly one sided PCB.   
Unfortunatelly I had to make some GND-connections to the second site to make the design some sort of clean.  

#### Partlist  
|Amount | Value | Designation
|-|-|-
| 1 | ESP32-WROOM-32 (ESP32) | ESP32 
| 1 | ER-TFTM032-3 | LCD 
| 1 | LD1117AS33TR (Voltage-Regulator) | IC1 
| 1 | SUMMER EPM 121 (buzzer) | SG1 
| 5 | 0,1µF | C1, C2, C4, C5, C6 
| 2 | 10µF | C3, C7 
| 4 | 10k | R1, R2, R3, R9 
| 1 | BC817 (NPN Transistor) | T1 
| 1 | Button | BTN 
| 3 | AAA Batteryholder | BT1, BT2, BT3  

As an optional accesory you can get a BME280 sensor module and connect it to the pinheader marked for it on the board.

### Case
It is an easy to print case.  
Probaly will make a new, improved version in the future.

## Pinout
|GPIO | Screen
|-|-
| 12 | MISO
| 13 | MOSI
| 14 | SCLK
| 15 | CS
| 2 | DC
| nc | RST
| 16 | T_SCL
| 27 | T_SDA

|GPIO | BME280
|-|-
|33|-
|25|-

|GPIO | Other
|-|-
|32| Button
|26| Speaker
|35| voltage divider

## Software
**W**ork **i**n **P**rogress

## Credits
[KGeri201](https://github.com/KGeri201)

Special thanks to [HimbeersaftLP](https://github.com/HimbeersaftLP) for the help.

## License
[Apache License 2.0](LICENSE)

## Project status
In development.
