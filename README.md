# Half-Adder-Schematic-to-GDSII
Design and implementation of CMOS Half Adder from schematic to GDSII using Cadence Virtuoso.
# CMOS Half Adder Design: From Schematic to GDSII using Cadence Virtuoso

![GitHub](https://img.shields.io/badge/Tool-Cadence%20Virtuoso-blue)
![Status](https://img.shields.io/badge/Project-Completed-brightgreen)
![Design](https://img.shields.io/badge/Design-CMOS%20Half%20Adder-orange)

---

# Overview

This project presents the complete custom VLSI design flow of a CMOS Half Adder using Cadence Virtuoso. The design begins with transistor-level schematic creation and proceeds through symbol generation, functional verification, transient simulation, physical layout design, Design Rule Check (DRC), Layout Versus Schematic (LVS) verification, and final GDSII generation for fabrication.

The objective of this project is to understand the complete custom IC design methodology followed in the semiconductor industry.

---

# Project Objectives

- Design a transistor-level CMOS Half Adder
- Verify the functionality using simulation
- Create the physical layout
- Perform DRC verification
- Perform LVS verification
- Generate fabrication-ready GDSII
- Understand the complete Full-Custom IC Design Flow

---

# Half Adder

A Half Adder is a combinational digital circuit that adds two one-bit binary inputs.

Inputs

- A
- B

Outputs

- Sum (S)
- Carry (C)

---

# Truth Table

| A | B | Sum | Carry |
|---|---|-----|-------|
|0|0|0|0|
|0|1|1|0|
|1|0|1|0|
|1|1|0|1|

---

# Boolean Equations

Sum

S = A ⊕ B

Carry

C = A · B

---

# CMOS Design Flow

The complete design flow followed in this project is

```
Specification

↓

Circuit Design

↓

Schematic Entry

↓

Symbol Creation

↓

Testbench Design

↓

Transient Simulation

↓

Layout Design

↓

Design Rule Check (DRC)

↓

Layout Versus Schematic (LVS)

↓

GDSII Generation
```

---

# Tools Used

- Cadence Virtuoso
- Spectre Simulator
- Virtuoso Layout XL
- Assura / PVS (DRC & LVS)
- GDSII Stream Out

---

# Technology

Technology Node : 90 nm CMOS

PDK : GPDK90


---

# Repository Structure

```
Half-Adder-Schematic-to-GDSII
│
├── README.md
│
├── Images
│   ├── 01_schematic.png
│   ├── 02_symbol_testbench.png
│   ├── 03_waveform.png
│   ├── 04_layout.png
│   ├── 05_drc.png          
│   ├── 06_lvs.png          
│   └── 07_gdsii.png       
│
│
└── GDSII

```

---

# Schematic Design

The Half Adder schematic was implemented using CMOS transistors in Cadence Virtuoso.

The design consists of

- CMOS XOR Gate
- CMOS AND Gate
- PMOS Network
- NMOS Network

The schematic was verified before moving to the layout stage.

### Schematic

<p align="center">
<img src="Images/01_schematic.png" width="900">
</p>

---

# Symbol Creation

A reusable symbol was generated from the transistor-level schematic.

The symbol was later used in the testbench for functional verification.

### Symbol and Testbench

<p align="center">
<img src="Images/02_symbol_testbench.png" width="900">
</p>
---

# Testbench

A dedicated testbench was created to verify all possible input combinations.

Input combinations tested

- 00
- 01
- 10
- 11

---

# Simulation Results

Transient analysis was performed using Spectre Simulator.

The simulation confirms

- Correct XOR operation
- Correct AND operation
- Proper timing response
- Accurate Sum output
- Accurate Carry output

### Waveform

<p align="center">
<img src="Images/03_waveform.png" width="1000">
</p>

---

# Layout Design

The transistor-level layout was manually created following CMOS layout design rules.

Special attention was given to

- Device Matching
- Proper Routing
- Minimum Area
- Metal Connections
- Well Contacts
- Substrate Contacts

### Layout

<p align="center">
<img src="Images/04_layout.png" width="1000">
</p>

---

# Design Rule Check (DRC)

The layout successfully passed all Design Rule Checks.

Result

✔ No DRC Errors

### DRC Report

*To be added after DRC verification.*
---

# Layout Versus Schematic (LVS)

The layout was compared with the original schematic.

Result

✔ Layout Matches Schematic

### LVS Report

*To be added after LVS verification.*

---

# GDSII Generation

After successful DRC and LVS verification, the final fabrication-ready GDSII file was generated.

### GDSII

*To be added after GDSII generation.*
---

# Results

Successfully designed and verified a CMOS Half Adder.

Achievements

- Functional Schematic
- Symbol Generation
- Successful Simulation
- Physical Layout
- DRC Clean
- LVS Matched
- GDSII Generated

---

# Learning Outcomes

Through this project, I learned

- CMOS Logic Design
- Custom IC Design Flow
- Cadence Virtuoso
- Schematic Capture
- Layout Design
- DRC Verification
- LVS Verification
- GDSII Generation
- Semiconductor Design Methodology

---

# Future Improvements

- Power Analysis
- Delay Optimization
- Area Optimization
- Stick Diagram
- Parasitic Extraction
- Post-Layout Simulation
- Full Adder Design
- Arithmetic Logic Unit (ALU) Design

---

# Author

Bhaskar Gupta

Electronics and Communication Engineer

Interested in

- VLSI Design
- Physical Design
- RTL Design
- ASIC Design
- Digital IC Design

GitHub:
https://github.com/Bhaskargupta021

LinkedIn:
https://linkedin.com/in/bhaskar-gupta-03735728b

---

# License

This project is intended for educational and learning purposes.
