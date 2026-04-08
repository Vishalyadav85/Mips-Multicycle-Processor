MIPS Multicycle Processor (Verilog)
Overview:

This project implements a MIPS Multicycle Processor using Verilog HDL. Unlike a single-cycle processor, this design executes each instruction over multiple clock cycles, improving hardware utilization and reducing complexity.

The processor supports core MIPS instructions and demonstrates concepts like control sequencing, ALU operations, memory access, and register file handling.

Features:
Multicycle execution of instructions
Efficient hardware reuse across cycles
Reduced clock cycle time compared to single-cycle design
Modular Verilog implementation
Supports key MIPS instructions:
R-type (add, sub, and, or, slt)
I-type (lw, sw, beq)
Jump (j)

Architecture:

The processor is divided into the following major components:

Datapath Components:

Program Counter (PC)
Instruction Register (IR)
Register File
ALU (Arithmetic Logic Unit)
Memory (Instruction + Data)
MDR (Memory Data Register)
A and B Registers (temporary registers)

Control Unit:
Finite State Machine (FSM)
Generates control signals based on instruction type and stage
 Execution Stages

Each instruction is executed in multiple steps:

Instruction Fetch (IF)
Instruction Decode (ID)
Execution (EX)
Memory Access (MEM)
Write Back (WB)

🛠️ Tools Used
Verilog HDL
Xilinx Vivado

The testbench:

Initializes clock and reset
Loads instructions into memory
Monitors outputs like:
PC value
ALU result
Register writes
Memory access
Sample Output
Correct execution of instructions over multiple cycles
Observable state transitions in waveform
Proper ALU operations and memory access

Learning Outcomes:
Understanding of multicycle CPU design
FSM-based control implementation
Efficient datapath utilization
Hands-on experience with Verilog simulation

Future Improvements:
Add pipeline implementation
Extend instruction set
Hazard detection and forwarding
Cache memory integration
