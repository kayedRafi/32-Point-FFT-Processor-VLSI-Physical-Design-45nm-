32-Point FFT Processor – VLSI Physical Design (45nm)

🚀 This project implements a 32-point Fast Fourier Transform (FFT) processor using a pipelined Radix-2 DIF (Decimation-In-Frequency) architecture, targeting 45nm technology (GPDK45).
The design demonstrates a complete RTL-to-GDSII ASIC implementation flow using Cadence EDA tools.

The goal of this project is to design a high-performance DSP hardware accelerator and implement it through the full VLSI physical design flow including synthesis, verification, and layout generation.

📌 Project Overview

Architecture: Radix-2 DIF Pipelined FFT

FFT Size: 32-point

Technology Node: GPDK 45nm

Design Type: ASIC Physical Design

Application: High-performance digital signal processing

The pipelined architecture improves throughput and allows continuous streaming of input data, making it suitable for real-time DSP applications.

⚙️ Design Flow

The project follows the standard RTL-to-GDSII ASIC design flow:

RTL Design

Verilog implementation of the 32-point FFT processor.

Logic Synthesis

Tool: Cadence Genus

RTL converted to gate-level netlist.

Logical Equivalence Check (LEC)

Tool: Cadence Conformal

Verified equivalence between RTL and synthesized netlist.

Physical Design

Tool: Cadence Innovus

Floorplanning

Standard cell placement

Clock Tree Synthesis (CTS)

Routing

Automation

Makefile flow used to automate synthesis-to-layout execution.

📊 Design Results
Parameter	Result
Gate Count	~59,070
Cell Count	~20,781
Core Area	~6066.5 µm²
Placement Density	~88%
Design Rule Violations	None

The design successfully passes physical design checks with no violations.

🛠 Tools Used

Cadence Genus – Logic synthesis

Cadence Conformal – Logical equivalence checking

Cadence Innovus – Physical design implementation

📂 Repository Structure
FFT-32-ASIC-Physical-Design
│
├── rtl/                # Verilog RTL source files
├── synthesis/          # Genus synthesis scripts
├── lec/                # Conformal LEC scripts
├── physical_design/    # Innovus flow scripts
├── reports/            # Timing, area, and power reports
├── results/            # Layout and design outputs
└── Makefile            # Automated design flow
📘 Applications

FFT processors are widely used in:

Digital Signal Processing (DSP)

Wireless Communication Systems

Image Processing

Audio Processing

Radar Systems

🎯 Learning Outcomes

Through this project, I gained practical experience in:

Complete RTL-to-GDSII ASIC design flow

Physical design implementation

DSP hardware accelerator architecture

EDA automation using Makefile

Working with 45nm technology node

🔗 Author

Kayed Ibnet


