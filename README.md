# Project PCB STM32F board

[![forthebadge](https://forthebadge.com/images/badges/built-with-love.svg)](https://forthebadge.com)

The PCB board is based on an STM32F microcontroller. It's similar to the ST Microelectronics Nucleo, which also features an STM32F. 

The board was realized on Altium Designer. It was produced by prototypist PCBway. This is a 4-layer PCB (top layer, GND layer, 3.3v layer and bottom layer) using vias.

*Project duration: 3 days*


# Table of contents
- [Electronic diagram](#schéma-électronique)
- [Routage de la Carte PCB](#routage-de-la-carte-pcb)
  

## Electronic diagram
The board's circuit diagram includes a two-pin male connector for the external power supply. This allows the board to be powered from 4 to 20 volts. A voltage regulator is used to convert the input voltage to 3.3V.

The middle of the page shows the STM32F microcontroller. It has 43 pins, 30 of which are GPIOS controllable. We use an external quartz oscillator to provide a stable frequency for this board.
The Reset pin on the microcontroller is connected to a pushbutton to reset the STM32F board.The STM32F has different boot options. The user is given the choice with a male connector.
The STM32F board has a JTAG (Joint Test Action Group) interface for testing, debugging and programming our board.

![alt text 1](st1.jpg) 

|  | Explanation |
|---------|---------|
| ![alt text 1](picture_ATtiny/carte_attiny.png) | L'objectif de la carte était de faire un design le plus petit possible : 17mm x 33 mm. Ceci permet d'avoir un coût pour une carte assez faible : 12 dollars chez PCBWay.Pour programmer la carte ATtiny nous aurons besoin d'une carte Arduino afin d'y installer le bootloader puis le programme dans l'ATtiny.|


## Routage de la Carte PCB

| Démonstration | Explication |
|---------|---------|
| ![alt text 1](picture_ATtiny/carte_attiny_2D.png) | La carte PCB est constitué de deux couches Top Layer et Bottom Layer. Nous avons un connecteur mâle en haut de la carte afin de programmer celle-ci. Pour cela on utilise le SPI de la carte ATtiny que l'on reliera au SPI de la carte Arduino. Nous avons ajouté le +5V et le GND afin de facilement alimenter la carte une fois celle-ci programmé.|
| ![alt text 1](picture_ATtiny/10-1.png) | j'ai ajouté deux connecteurs femelles de part et d'autres de l'ATtiny afin de facilement relier des composants à celle-ci. |


## Arduino Factory

 * [Plus de détails sur le projet](https://arduinofactory.fr/carte-pcb-attiny/)
  





