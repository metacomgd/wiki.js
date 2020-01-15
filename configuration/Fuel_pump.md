---
title: Fuel pump
description: Setting the on/off conditions of the fuel pump
published: true
date: 2020-01-14T06:24:04.641Z
tags: aux outputs, tuning
---

# Header
Fuel pump ontrol is a simple but important function performed by the ECU. Currently Speeduino does not perform variable (PWM) pump control, but 

## Settings
![fuel_pump.png](/img/accessories/fuel_pump.png =500x){.align-center}

* **Fuel pump pin** - The Arduino pin that the fuel pump output is on. In most cases this should be left to `Board Default` unless you have a specific reason to change this. 
* **Prime duration** - How long (In seconds) the fuel pump should run when the system is first powered up. Note that this is triggered **when the ECU is powered on**, which will not always be the same as when the ignition is turned out. If you have a USB cable connected then the ECU is already powered up. 