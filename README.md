# RISC-V---CALCULATOR

📘 RISC-V Pipeline Simulation Project
📌 Project Overview

This project demonstrates the execution of a RISC-V assembly program using the Ripes Simulator. It focuses on understanding the instruction pipeline (IF, ID, EX, MEM, WB stages), hazards, and how instructions flow through the processor.

🎯 Objectives

To learn the basics of RISC-V assembly programming.

To visualize how instructions are executed in a 5-stage pipeline.

To analyze hazards such as data dependency and stalls.

To understand the internal working of RISC-V processors through simulation.

🛠️ Tools & Requirements

Ripes Simulator (GUI tool for RISC-V visualization)

RISC-V assembly code (example provided)

Windows/Linux/Mac OS

📂 Project Description

The program loads values from memory, performs arithmetic operations (add, sub, mul, div), and uses the pipeline diagram to show how instructions overlap in execution.

Sample Code Executed:
auipc x5, 0x10000  
addi x5, x5, 0  
lw x6, 0(x5)  
auipc x5, 0x10000  
addi x5, x5, -8  
lw x7, 0(x5)  
add x28, x6, x7  
sub x29, x6, x7  
mul x30, x6, x7  
div x31, x6, x7  
ecall

Pipeline Stages Observed:

IF (Instruction Fetch)

ID (Instruction Decode)

EX (Execute)

MEM (Memory Access)

WB (Write Back)

📊 Expected Output

A pipeline diagram showing the overlapping of instructions.

Identification of hazards (stall cycles, dependencies).

Execution result of arithmetic operations.

🚀 Applications

Useful for students & beginners to understand processor design.

Can be extended into projects like:

Hazard detection units

Forwarding mechanism simulation

Custom instruction design in RISC-V

👨‍💻 Author

VISHALI R (v7shali)
