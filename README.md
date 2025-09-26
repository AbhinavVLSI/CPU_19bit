# CPU_19bit

A 5-stage pipelined RISC processor implemented in Verilog, featuring data forwarding, hazard detection, and a custom instruction set.

📖 About The Project
This project is a complete implementation of a 5-stage pipelined CPU from scratch in Verilog HDL. The architecture is designed for efficiency, mitigating common pipeline hazards through dedicated hardware units. It's a great project for understanding the core principles of computer architecture, including instruction set design, pipelining, data dependencies, and control logic.

The pipeline is structured into the following five stages:

IF (Instruction Fetch): Fetches the next instruction from memory.

ID (Instruction Decode): Decodes the instruction, reads operands from the register file, and generates control signals.

EX (Execute): Performs calculations in the ALU.

MEM (Memory Access): Reads from or writes to data memory.

WB (Write Back): Writes the result back into the register file.

✨ Features
5-Stage Pipelined Design: Classic RISC pipeline for parallel instruction execution.

Data Hazard Resolution: A forwarding_unit resolves data hazards without stalling the pipeline in most cases.

Control & Load-Use Hazard Detection: A hazard_unit flushes the pipeline on branches/jumps and stalls for load-use hazards to ensure correct execution.

Custom RISC ISA: A custom instruction set architecture (ISA) with support for:

Arithmetic (ADD, SUB, MUL, DIV, INC, DEC)

Logical (AND, OR, XOR, NOT)

Memory (LD, ST)

Control Flow (JMP, BEQ, BNE, CALL, RET)

Specialized Instructions: Includes custom opcodes for FFT, ENC (Encryption), and DCRPT (Decryption) to showcase extensibility.

16 x 32-bit Register File: A general-purpose register file for data manipulation.

🚀 Getting Started
To get a simulation of this CPU running, you'll need a Verilog simulator.
