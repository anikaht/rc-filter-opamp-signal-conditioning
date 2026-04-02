# RC Filter + Op-Amp Signal Conditioning

## Overview
Designed a basic analog signal-conditioning circuit using a first-order RC low-pass filter and a non-inverting op-amp amplifier.

## Tools
- LibrePCB
- Ngspice

## Circuit
- R1 = 10kΩ
- C1 = 0.1µF
- R2 = 100kΩ
- R3 = 10kΩ

## Results
AC simulation shows:
- ~20 dB passband gain
- cutoff near 159 Hz
- attenuation of higher-frequency noise

## Files
- `schematic.png`
- `schematic.pdf`
- `response.png`
- `rc_opamp.cir`
