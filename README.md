# 32-bit Universal Shift Register

> Digital Logic → PCB Design → Hardware Implementation

### Digital Logic Design

![Logisim Circuit](Images/01_Logisim.png)

### Schematic

![Schematic](Images/02_Schematic.png)

### PCB Layout

![PCB Layout](Images/03_PCB_Layout.png)

### 3D PCB View

![3D PCB View](Images/04_3D_View.png)



## Overview

This project demonstrates the complete engineering workflow of designing and implementing a **32-bit Universal Shift Register**, beginning with digital logic simulation in **Logisim Evolution** and progressing to physical PCB design in **KiCad**.

The project was developed using a modular approach. A reusable **4-bit Universal Shift Register module** was first designed, verified, and optimized before being expanded into a complete **32-bit architecture**. This methodology simplified debugging, improved design verification, and created a scalable hardware solution.

Throughout the project, emphasis was placed not only on implementing the required functionality—**Hold, Shift Left, Shift Right, and Parallel Load**—but also on understanding the engineering process behind digital hardware development, including logic verification, schematic capture, PCB layout, routing, ground plane design, and Design Rule Checking (DRC).

The final PCB successfully passed **KiCad Design Rule Checking (DRC) with zero errors**, demonstrating that the design is electrically consistent and ready for fabrication.

## Features

- Implements a complete **32-bit Universal Shift Register** architecture.
- Supports all four fundamental operations:
  - Hold
  - Shift Left
  - Shift Right
  - Parallel Load
- Designed using a **modular 4-bit architecture** for scalability and easier verification.
- Digital logic designed and validated in **Logisim Evolution** before hardware implementation.
- Complete schematic capture and PCB layout developed in **KiCad**.
- Two-layer PCB with organized component placement and copper routing.
- Ground plane implementation for improved PCB design practices.
- Successfully passed **KiCad Design Rule Check (DRC)** with **zero errors**.
- Ready for PCB fabrication through generated **Gerber** and **Drill** files.

## System Architecture

The project follows a modular architecture in which a reusable **4-bit Universal Shift Register module** serves as the fundamental building block of the complete system. The project follows a modular architecture in which a reusable **4-bit Universal Shift Register PCB module** serves as the fundamental building block of the complete system. The module is designed to be replicated **eight times**, allowing the construction of a complete **32-bit Universal Shift Register** while simplifying verification, debugging, and future hardware expansion.

### Design Flow

```text
Digital Logic Design (Logisim Evolution)
                │
                ▼
      4-bit Universal Shift Register
                │
                ▼
      Verification & Debugging
                │
                ▼
      Schematic Design (KiCad)
                │
                ▼
      PCB Layout & Routing
                │
                ▼
      Ground Plane & DRC Verification
                │
                ▼
      Gerber & Drill File Generation
                │
                ▼
     32-bit Hardware Implementation
```

## PCB Design

The PCB was designed using **KiCad** after completing and verifying the digital logic in **Logisim Evolution**. The objective was to transform the simulated design into a manufacturable hardware module while following good PCB design practices.

The PCB development process included:

- Schematic capture
- Footprint assignment
- Component placement
- Signal routing
- Ground plane implementation
- Design Rule Checking (DRC)
- 3D model verification
- Gerber and Drill file generation

The final PCB successfully passed **KiCad Design Rule Checking (DRC)** with **zero errors**, confirming that the design satisfies the defined electrical and manufacturing rules before fabrication.

## Design Challenges

One of the most significant challenges during this project occurred during the digital logic design phase. While testing the custom logic implementation, some multiplexer select states did not operate as expected. Instead of redesigning the circuit immediately, the logic was analyzed systematically at the gate level to identify the root cause. The issue was traced to an incorrect decode stage, and after correcting the logic, all four operating modes functioned correctly.

Another challenge was transitioning from digital simulation to PCB design. This required learning schematic capture, footprint assignment, component placement, PCB routing, copper pours, and manufacturing file generation using KiCad. Careful verification throughout the design process ensured that the final PCB passed **Design Rule Checking (DRC)** with **zero errors** and was prepared for fabrication.

This project reinforced the importance of systematic debugging, verification before implementation, and careful PCB design practices when transforming a digital logic design into hardware.

## Results

The project successfully demonstrates the complete design workflow of a **32-bit Universal Shift Register**, progressing from digital logic simulation to PCB implementation.

### Achievements

- Successfully designed and verified the digital logic in **Logisim Evolution**.
- Developed a reusable **4-bit Universal Shift Register PCB module** that can be replicated to construct a complete **32-bit Universal Shift Register**.
- Completed the complete schematic and PCB layout using **KiCad**.
- Successfully implemented all required Universal Shift Register operations:
  - Hold
  - Shift Left
  - Shift Right
  - Parallel Load
- Generated manufacturing-ready **Gerber** and **Drill** files.
- Successfully passed **KiCad Design Rule Checking (DRC)** with **zero errors**.
- Verified the PCB design using KiCad's integrated **3D Viewer**.

## Repository Structure

```text
32-bit-Universal-Shift-Register/
│
├── Documentation/     # Project report and documentation
├── Images/            # Screenshots and PCB renders
├── KiCad/             # KiCad project files
├── Logisim/           # Logisim simulation files
├── Gerber/            # Manufacturing (Gerber & Drill) files
├── Datasheets/        # Component datasheets
├── Videos/            # Project demonstration videos
└── README.md          # Project overview
```

## Future Improvements

While the project successfully demonstrates the complete design workflow from digital logic simulation to PCB implementation, several enhancements can be incorporated in future revisions.

Potential improvements include:

- Manufacture and assemble the PCB for hardware validation.
- Experimentally verify all operating modes using physical testing.
- Optimize component placement and routing for improved PCB organization.
- Reduce the overall board size while maintaining signal integrity.
- Minimize the number of vias where practical to simplify manufacturing.
- Extend the modular architecture to support larger digital systems.
- Explore modern logic families or programmable devices such as CPLDs or FPGAs for higher-speed implementations.

## Author

### Natasha Eman

**BS Electrical Engineering Student**  
FAST National University (NUCES), Pakistan

### Areas of Interest

- Digital Hardware Design
- PCB Design
- Embedded Systems
- Computer Vision
- Embedded AI

### Technologies & Tools

- KiCad
- Logisim Evolution
- Python
- OpenCV
- Git & GitHub

---

This project represents my journey from digital logic simulation to PCB implementation, with the goal of strengthening my understanding of practical hardware design and engineering workflows.

I welcome constructive feedback and suggestions for improving both the design and the documentation.