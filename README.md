
# Solar PV Fed Buck-Boost Converter Based BLDC Motor for Air Cooler Application

## 📖 Overview

This repository presents a comprehensive design and performance analysis of a 1000 W solar photovoltaic (PV)-fed Brushless DC (BLDC) motor drive. The system is specifically optimized for cooling infrastructure, efficiently driving dual mechanical load sinks: a water pump and a blower fan.

To overcome the challenge of non-linear PV output under fluctuating environmental conditions, the architecture integrates a DC-DC Buck-Boost converter regulated by a Perturb and Observe (P&O) Maximum Power Point Tracking (MPPT) algorithm. The BLDC motor itself is driven by a three-phase Voltage Source Inverter (VSI) utilizing electronic commutation derived from Hall-effect sensor feedback.


## ✨ Key Features

* 
**Dynamic MPPT Tracking:** Employs a P&O logic loop to constantly sample, perturb, and actuate the system, locking onto the shifting Maximum Power Point (MPP) during irradiation transients (e.g., sudden cloud cover dropping irradiance from 1000 W/m² to 400 W/m²).


* 
**Robust Power Conversion:** A Buck-Boost converter acts as an impedance-matching power buffer, stepping voltage up or down to ensure optimal energy extraction regardless of terminal load conditions.


* 
**Precise Commutation Logic:** Utilizes 120-degree conduction mode logic to decode physical Hall sensor data into Back-EMF references, generating perfectly timed discrete gate pulses for the VSI.


* 
**Dual Load Management:** Independently manages the stator current profiles, Back-EMF transients, and torque/speed feedback for both a centrifugal water pump and a blower fan.



## ⚙️ System Configuration & Parameters

The hardware sizing and software parameters modeled in MATLAB/Simulink are detailed below:

* 
**Total PV Array Capacity:** 1000 W (Scaled using four 250 W monocrystalline panels connected in series).


* 
**Open-Circuit Baseline / Total PV String Voltage:** ~122 V.


* 
**Maximum Power Voltage per Panel:** 30.5 V.


* 
**DC-DC Converter Type:** Buck-Boost Converter.


* 
**MPPT Algorithm:** Perturb and Observe (P&O).


* 
**Inverter Type:** Three-phase Voltage Source Inverter.


* 
**Motor Commutation Method:** 120-degree Hall sensor-based.



## 📊 Simulation & Results

The MATLAB/Simulink environment was used to inject a precise, stepped simulation stress-test profile (1000 W/m² → 400 W/m² → 700 W/m² → 1000 W/m²).

* Steady-state simulations confirm that the optimized P&O step size completely eliminates power oscillation, locking precisely onto the maximum extraction limit.


* During aggressive environmental drops, the system safely absorbs electrical transients, allowing BLDC stator current and motor torque to re-stabilize safely at lower power thresholds.



## 🔗 Resources & Links

* 
**Video Demonstration:** [Watch the full simulation results on YouTube](https://www.youtube.com/watch?v=shTebeWrGZ8).

  [![Watch the simulation on YouTube](https://img.youtube.com/vi/shTebeWrGZ8/maxresdefault.jpg)](https://www.youtube.com/watch?v=shTebeWrGZ8)


* 
**Purchase the Model:** [LMS Solution Product Page (SKU: 0032)](https://www.lmssolution.net.in/product-page/solar-pv-fed-buck-boost-converter-based-bldc-motor-for-air-cooler-application).

[![Purchase Model](https://img.shields.io/badge/Purchase_Model-SKU_0032-238636?style=for-the-badge)](https://www.lmssolution.net.in/product-page/solar-pv-fed-buck-boost-converter-based-bldc-motor-for-air-cooler-application)


[![Get the MATLAB Model](model-image.png)](https://www.lmssolution.net.in/product-page/solar-pv-fed-buck-boost-converter-based-bldc-motor-for-air-cooler-application)



* 
**Support:** For inquiries, contact `support@lmssolution.net` or `info@lmssolution.net.in`.
