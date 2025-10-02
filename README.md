# FPGA I²C Address Translator

This project implements an **I²C address translator on FPGA**.  
It allows a master device to communicate with a target I²C device using a **remapped virtual address**, solving address conflicts.

## Features
- Acts as I²C Slave (to bus master) and I²C Master (to target device).
- Translates one target address at a time.
- Supports bidirectional read/write.
- FSM + shift-register design for FPGA efficiency.
- Verified using simulation on [EDA Playground](https://edaplayground.com).

## Repository Layout
- `src/` → Verilog source and testbench.
- `sim/` → Simulation files & EDA Playground link.
- `reports/` → FPGA synthesis resource report.
- `docs/` → Architecture documentation.

## How to Run Simulation
1. Open [EDA Playground](https://edaplayground.com).
2. Load `i2c_addr_translator.v` and `tb_i2c_translator.v`.
3. Run using **Icarus Verilog + GTKWave**.
4. Check output & waveform.

## Example Simulation Output
