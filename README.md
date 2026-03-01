# 555 Astable Multivibrator – Design, Simulation, PCB & Hardware Implementation

## 📌 Project Overview

This project demonstrates the complete engineering workflow of designing and implementing a **555 Timer in Astable Mode**, including:

- Schematic Design (KiCad)
- 2-Layer PCB Design with Ground Plane
- LTspice Simulation & Waveform Verification
- Hardware Implementation & Testing

The circuit generates a continuous square wave output without any external triggering signal.

---

## ⚙️ Circuit Description

The NE555 timer is configured in astable mode, where it continuously oscillates between HIGH and LOW output states.

The timing capacitor charges and discharges between:

- 1/3 Vcc
- 2/3 Vcc

This process produces a square wave output.

A diode is included to allow independent control of charging and discharging paths, enabling duty cycle adjustment.

---

## 📐 Design Parameters

- Supply Voltage: 5V
- R1 = 9kΩ
- R2 = 9kΩ
- C = 0.01µF
- Control Voltage Capacitor = 0.01µF
- Diode for duty cycle control

---

## 🔢 Theoretical Calculations

Charging Time:
TH = 0.693 × R1 × C  

Discharging Time:
TL = 0.693 × R2 × C  

Total Period:
T = TH + TL  

Frequency:
f = 1 / T  

For the selected values:

Frequency ≈ 8 kHz  
Duty Cycle ≈ 50%

The calculated values match the simulation and hardware results.

---

## 🛠 Tools Used

- KiCad – Schematic & PCB Design
- Design Rule Check (DRC)
- Gerber & Drill File Generation
- LTspice – Circuit Simulation
- Oscilloscope – Hardware Waveform Measurement

---

## 🔥 PCB Features

- 2-layer PCB (F.Cu & B.Cu)
- Full GND copper plane on bottom layer
- Thermal relief pad connections
- Clean routing with proper clearance
- DRC verified (0 errors)
- Through-hole component layout

---

## 📊 Simulation Results (LTspice)

- Stable square wave output
- ~8 kHz frequency
- ~50% duty cycle
- Output swing: 0V to 5V

Simulation results match theoretical calculations.

---

## 🔬 Hardware Implementation

The circuit was assembled and tested using:

- NE555 IC
- 5V regulated power supply
- Measured using oscilloscope

Observed Results:

- Stable square wave output
- Frequency close to calculated value
- Proper duty cycle
- Reliable oscillation

This confirms the correctness of the design from simulation to real-world implementation.

---

## 📁 Repository Contents

- KiCad Schematic Files
- PCB Layout Files
- 3D Board View
- LTspice Simulation File (.asc)
- Hardware Images
- Oscilloscope Output Screenshot

---

## 🎯 Learning Outcomes

- Analog timing circuit design
- Practical PCB layout techniques
- Ground plane implementation
- SPICE simulation and waveform verification
- Frequency and duty cycle analysis
- End-to-end hardware validation

---

## 👨‍💻 Author

Dhanush S Poojary  
Electronics & Communication Engineering  
AEC Project – 555 Timer Astable Design

## 👨‍💻 Author

Dhanush S Poojary  
Electronics & Communication Engineering  
AEC Project – 555 Astable Timer Design
