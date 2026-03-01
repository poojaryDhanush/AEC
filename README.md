# 555 Astable Multivibrator – Complete Design & Simulation

## 📌 Project Overview

This project presents the complete design, simulation, and PCB implementation of a **555 Timer configured in Astable Mode**.

The project includes:

- Schematic design using **KiCad**
- 2-layer PCB layout with ground plane
- LTspice simulation with waveform verification
- Fabrication-ready Gerber files

The circuit generates a continuous square wave output without external triggering.

---

## ⚙️ Circuit Description

The NE555 timer is configured in **astable mode**, where it continuously switches between HIGH and LOW states.

The capacitor charges and discharges between:

- 1/3 Vcc
- 2/3 Vcc

This charging/discharging action produces a square wave at the output.

---

## 📐 Design Parameters

- Supply Voltage: 5V
- R1 = 9kΩ
- R2 = 9kΩ
- C = 0.01µF
- Control Voltage Capacitor = 0.01µF
- Diode added for duty cycle control

---

## 🔢 Frequency Calculation

For diode-modified astable:

TH = 0.693 × R1 × C  
TL = 0.693 × R2 × C  

Total Period:

T = TH + TL  

Frequency:

f = 1 / T  

For the selected values:

f ≈ 8 kHz  
Duty Cycle ≈ 50%

---

## 🛠 Tools Used

- KiCad (Schematic & PCB Design)
- Design Rule Check (DRC)
- Gerber Generation
- LTspice (Waveform Simulation)

---

## 🔥 PCB Features

- 2-layer PCB (F.Cu & B.Cu)
- Full GND copper plane on bottom layer
- Thermal relief pad connections
- Clean routing with proper clearance
- DRC verified (0 errors)
- Fabrication-ready Gerber files
- Through-hole component layout

---

## 📊 Simulation Results

The LTspice simulation confirms:

- Stable square wave output
- Approximate 8 kHz frequency
- Nearly 50% duty cycle
- Output swing from 0V to 5V

Waveform verification matches theoretical calculations.

---

## 📁 Repository Contents

- KiCad Schematic Files
- PCB Layout Files
- 3D Board View
- LTspice Simulation File (.asc)
- Output Waveform Screenshot

---

## 🎯 Learning Outcomes

- Practical PCB design workflow
- Ground plane implementation
- Netlist & DRC validation
- Hardware timing analysis using 555
- SPICE-based simulation verification
- Frequency and duty cycle calculation

---

## 👨‍💻 Author

Dhanush S Poojary  
Electronics & Communication Engineering  
AEC Project – 555 Astable Timer Design
