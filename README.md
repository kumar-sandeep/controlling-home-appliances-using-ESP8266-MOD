# Welcome to my page

## Table of Contents
* [Introduction](#introduction)
* [Aim and Objective](#aim-and-objective)
* [Expected outcome](#expected-outcome)
* [Materials Required](#materials-required)
  * [Wifi Module](#wifi-module)
  * [Relay Module](#relay-module)
  
  
## Introduction
In this project we are going to make a home automation system using ESP8266 Wi-Fi module. Using this we will be able to control lights, electric fan and other home appliances through a web browser using our PC or mobile. These AC mains appliances will be connected to relays which are controlled by the ESP8266. ESP8266 acts as a Web Server and we will send control commands through a Web Browser like Google Chrome or Mozilla Firefox. ESP8266 is the one of the most popular and low cost Wi-Fi module available in the market today.

## Aim and Objective
The main Objective of our work is to automate the Home Appliances using Android Application or the Computer, basically the project is very much important for Specially challenged People who are unable to go everywhere every time to control the home appliances, for that they can be in one position and can control the home appliances.

Also for the people who are sleeping at night and are feeling lazy to either switch off/on the fan or A.C. or any of the home appliances they can turn on/off using there android phone.

Some times in this busy world people generally forget to switch off there fan or light or any home appliance in hurry while leaving home in that case they can also turn on/off it after leaving the home using there Android Application.

Also, for the parents who fear of getting electric shocks if their children use the switch, then in that case too our project work is very useful as the child can control the home appliances using the Android Application and is safe for electric shocks.


## Expected outcome
The home appliances can be controlled with any android mobile or web browser anywhere, anytime. 
The user will have application which will allow easier operation of wifi module.
And also a webpage which will control over wifi module, if not have android mobile.
It can be controlled with any computer.

# Materials Required

## Wifi Module
<img src="./wifi.png" alt="wifi.png" width="350">
This is a Wi-Fi module which we are using in our project. Its model is “Esp8266mod” and vendor is “Ai-Thinker”. It’s an impressive, low cost Wi-Fi module suitable for adding Wi-Fi functionality to an existing microcontroller project via a UART serial connection. The module can even be reprogrammed to act as a standalone Wi-Fi connected device–just add power.

### Configuration of esp module
1.	Input Voltage = 5v
2.	Output Voltage=3.3v
3.	It has 16 GPIO pins,can be used for both input and output.
4.	It can be used as standalone module i.e no additional programmer needed to program this board.
5.	It can work in 3 modes
i)	Station Mode  :	It can connect to existing Wi-Fi Access Points.
ii)	Soft-AP Mode:	It can create Wi-Fi Access Points.
iii)	It is also able to operate both in station mode and soft Access Point Mode at the same point.

### why this module
1.Fully integrated module i.e inbuilt with programmer.
2.Can be powered by any usb cable mobile charger.
3.Easily programmed by using Arduino IDE.
4.Very low Power consumption.
5.Cost Effective.
6.Easily available in Online Shopping websites such as Amazon and Ebay.

### Pin diagram of esp
<img src="./pinDiagram.png" alt="pinDiagram.png" width="350">


## Relay Module
This is a relay module having 4 5v relays.

### Configuration of relay Module
1.	Input Voltage:	5v.
2.	Input Current:	15-20mA .Each of the 4 relays shown above needs 15-20 mA driver current.
3.	Output Voltage:	 220v AC.
4.	Output current  :	upto 10A

### What is a relay?
We know that most of the high end industrial application devices have relays for their effective working. Relays are simple switches which are operated both electrically and mechanically. Relays consist of a n electromagnet and also a set of contacts. The switching mechanism is carried out with the help of the electromagnet. There are also other operating principles for its working. But they differ according to their applications. Most of the devices have the application of relays.

### Why is a relay used?
The main operation of a relay comes in places where only a low-power signal can be used to control a circuit. It is also used in places where only one signal
can be used to control a lot of circuits.
Here we are using dc voltages in module and we are trying to connect and switch AC devices using signals sent by the Wi-Fi module. So here comes the application of relay.

### Relay Design
There are only four main parts in a relay. They are
	Electromagnet
	Movable Armature
	Switch point contacts
	Spring
The figures given below show the actual design of a simple relay.

<img src="./relayConstruction.png" alt="relayConstruction.png" width="350">
It is an electro-magnetic relay with a wire coil, surrounded by an iron core. A path of very low reluctance for the magnetic flux is provided for the movable armature and also the switch point contacts.  The movable armature is connected to the yoke which is mechanically connected to the switch point contacts. These parts are safely held with the help of a spring. The spring is used so as to produce an air gap in the circuit when the relay becomes de-energized.

### How relay works?
The working of a relay can be better understood by explaining the following diagram given below.

<img src="./relayDesign.png" alt="relayDesign.png" width="350">

The diagram shows an inner section diagram of a relay. An iron core is surrounded by a control coil. As shown, the power source is given to the electromagnet through a control switch and through contacts to the load. When current starts flowing through the control coil, the electromagnet starts energizing and thus intensifies the magnetic field. Thus the upper contact arm starts to be attracted to the lower fixed arm and thus closes the contacts causing a short circuit for the power to the load. On the other hand, if the relay was already de-energized when the contacts were closed, then the contact move oppositely and make an open circuit.
As soon as the coil current is off, the movable armature will be returned by a force back to its initial position. This force will be almost equal to half the strength of the magnetic force. This force is mainly provided by two factors. They are the spring and also gravity.
Relays are mainly made for two basic operations. One is low voltage application and the other is high voltage. For low voltage applications, more preference will be given to reduce the noise of the whole circuit. For high voltage applications, they are mainly designed to reduce a phenomenon called arcing.

### Relay Basics

The basics for all the relays are the same. Take a look at a 4 – pin relay shown below. There are two colours shown. The green colour represents the control circuit and the red colour represents the load circuit. A small control coil is connected onto the control circuit. A switch is connected to the load. This switch is controlled by the coil in the control circuit. Now let us take the different steps that occour in a relay.

<img src="./relayDesign.png" alt="relayDesign.png" width="350">

### Energized Relay (ON)

As shown in the circuit, the current flowing through the coils represented by pins 1 and 3 causes a magnetic field to be aroused. This magnetic field causes the closing of the pins 2 and 4. Thus the switch plays an important role in the relay working. As it is a part of the load circuit, it is used to control an electrical circuit that is connected to it. Thus, when the relay in energized the current flow will be through the pins 2 and 4.

<img src="./relayOn.png" alt="relayOn.png" width="350">

### De-Energized Relay (OFF)

As soon as the current flow stops through pins 1 and 3, the switch opens and thus the open circuit prevents the current flow through pins 2 and 4. Thus the relay becomes de-energized and thus in off position.

<img src="./relayOff.png" alt="relayOff.png" width="350">

*In simple, when a voltage is applied to pin 1, the electromagnet activates, causing a magnetic field to be developed, which goes on to close the pins 2 and 4 causing a closed circuit. When there is no voltage on pin 1, there will be no electromagnetic force and thus no magnetic field. Thus the switches remain open*


## Breadboard

<img src="./breadboard.png" alt="breadboard.png" width="350">

A breadboard is a construction base for prototyping of electronics.


## Jumper Wire

<img src="./jumperWire.png" alt="breadboard.png" width="350">

Jumper wires are the connecting wire which are breadboard and relay friendly.
They are of three types 
i)	Female to female 
ii)	Male to male 
iii)	Female to male 


## Resistor

<img src="./resistor.png" alt="resistor.png" width="350">

Two resistances are needed in our project.
1)	47K 
2)	1K


## Transistor bc547

<img src="./bc547transistor.png" alt="bc547transistor.png" width="350">

BC547 is an NPN Bi-polar junction transistor (BJT) as shown in figure. A transistor, stands for transfer of resistance, is commonly used to amplify current. A small current at its base controls a larger current at collector & emitter terminals.
Together with other electronic components, such as resistors, coils, and capacitors, it can be used as the active component for switches and amplifiers. 


## Dedicated Power Supply for the Relay

<img src="./dedicatedPowerSupplyForRelay.png" alt="dedicatedPowerSupplyForRelay.png" width="350">

The above is the dedicated power supply circuit and the 9v dc adapter, the 9v adapter is plugged into the circuit and the circuit can give output of 5v and 3.3v and its current is sufficient enough to trigger 5v relay. It can be easily purchased from amazon and eBay.


## 3v to 5v switch

<img src="./3vto5vSwitch.png" alt="3vto5vSwitch.png" width="350">

Above is a circuit diagram of 3v to 5v switch.
The left end is coming from Wi-Fi module.


## How to Setup Hardware

<img src="./hardwareSetup.png" alt="hardwareSetup.png" width="350">

Working with 5v Relay using 3.3v signal from esp module.The figure 2 shows the pin configuration of figure 1 in complete.

<img src="./completeHardwareSetup.png" alt="completeHardwareSetup.png" width="350">

*Figure 3 shows the complete setup of relays, Wi-Fi module and connectivity with home appliances.*
Relays and appliances are connected with ac supply (220v). Wi-Fi module is connected with any 5v DC supply through usb. The relays should be given a power supply of 5v dc sufficient enough to trigger the relay coil and make it work. The states of Relays are normally open. When the on signal is received, the relay switches to normally closed state and appliances are turned on.




