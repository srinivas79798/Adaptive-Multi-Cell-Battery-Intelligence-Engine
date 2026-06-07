# Adaptive Multi-Cell Battery Intelligence Engine

## Overview

The Adaptive Multi-Cell Battery Intelligence Engine is an ESP32-based Battery Management System (BMS) designed to monitor a simulated 4-cell lithium-ion battery pack in real time. The system continuously measures individual cell voltages, calculates battery pack statistics, detects cell imbalance, and classifies battery health conditions.

## Features

* Real-time monitoring of 4 battery cells
* Individual cell voltage measurement
* Average pack voltage calculation
* Strongest and weakest cell identification
* Cell imbalance percentage calculation
* Battery health classification:

  * Healthy
  * Minor Imbalance
  * Critical Imbalance
  * Pack Failure
* Fault indication using LEDs
* Audible alerts using a buzzer
* Relay control for battery protection
* IoT dashboard integration using Blynk
* LCD display for local monitoring

## Hardware Components

* ESP32 Development Board
* LCD 16x2 I2C Display
* LEDs (Red, Yellow, Green)
* Buzzer
* Relay Module
* Simulated Battery Cell Inputs
* Wi-Fi Connectivity

## Software Used

* Arduino IDE
* Embedded C/C++
* Blynk IoT Platform
* ESP32 Libraries

## Working Principle

The ESP32 reads voltage values from four battery cells through ADC pins. The system calculates the average voltage, determines the highest and lowest cell voltages, and computes the imbalance percentage. Based on predefined thresholds, the battery pack is classified into different health states. The results are displayed on an LCD screen and transmitted to the Blynk cloud dashboard for remote monitoring.

## Battery Health Conditions

| Condition          | Criteria                    |
| ------------------ | --------------------------- |
| Healthy            | Imbalance ≤ 10%             |
| Minor Imbalance    | Imbalance > 10%             |
| Critical Imbalance | Imbalance > 25%             |
| Pack Failure       | Minimum Cell Voltage < 1.0V |

## Output Parameters

* Cell 1 Voltage
* Cell 2 Voltage
* Cell 3 Voltage
* Cell 4 Voltage
* Average Pack Voltage
* Maximum Cell Voltage
* Minimum Cell Voltage
* Strongest Cell
* Weakest Cell
* Imbalance Percentage
* Battery Status

## Applications

* Electric Vehicle Battery Monitoring
* Energy Storage Systems
* Solar Battery Management
* Industrial Battery Packs
* IoT-Based Battery Diagnostics

## Author

Sudanapalli Srinivas

Bachelor of Technology (ECE)


