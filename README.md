# RC Filter + Op-Amp Signal Conditioning Circuit

## Overview
This project demonstrates a basic analog signal conditioning circuit using a first-order RC low-pass filter and a non-inverting op-amp amplifier.

The design filters out high-frequency noise from a sensor signal and amplifies the useful signal before it is processed by an embedded system (e.g., ADC input).

---

## Tools Used
- LibrePCB (schematic design)
- Ngspice (AC simulation)

---

## Circuit Design

- R1 = 10kΩ, C1 = 0.1µF → low-pass filter  
- R2 = 100kΩ, R3 = 10kΩ → non-inverting amplifier  

### Key Characteristics
- Cutoff frequency:
  - Theoretical:  
    \( f_c = \frac{1}{2\pi RC} \approx 159 \, \text{Hz} \)
- Gain:
  - \( 1 + \frac{R2}{R3} = 11 \) (~20 dB)

---

## Schematic
![Signal Conditioning Schematic](signal-conditioning-schematic.png)

---

## Simulation (AC Analysis)
![AC Response Plot](ac-response-plot.png)

### Results
- Passband gain ≈ 20 dB (~11× amplification)
- Cutoff frequency ≈ 159 Hz (matches theoretical calculation)
- High-frequency signals are attenuated as expected from a low-pass filter

---

## Why This Project Matters
This project demonstrates a complete analog design workflow:

- Designing a signal-conditioning circuit for sensor inputs  
- Selecting component values based on desired frequency response  
- Simulating behavior using Ngspice  
- Validating theoretical expectations with simulation results  

Such circuits are commonly used in:
- Sensor signal conditioning  
- Embedded systems (pre-ADC filtering)  
- Wearable and IoT devices  

---

## Files
- `signal-conditioning-schematic.png` → circuit diagram  
- `ac-response-plot.png` → frequency response plot  
- `rc_opamp.cir` → Ngspice simulation file  
- `schematic.pdf` → schematic export  

---

## Summary
This project validates a simple but widely used analog front-end design that combines filtering and amplification, forming a foundation for more advanced embedded and sensing systems.
