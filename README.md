# Instruction-Set-Design-RISC-V

# RISC-V 32-bit CPU Model and ISA

## Table of Contents

- [Description](#description)
- [Tools Used](#tools-used)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgements](#acknowledgements)

## Description

Welcome to this project! This is a **RISC-V 32-bit CPU Model and Instruction Set Architecture (ISA)** design project. The goal is to create a custom instruction set based on the RISC-V architecture and implement a CPU model capable of performing arithmetic, logical, load/store, and branch operations. The project involves designing the CPU datapath, control signals, and instruction mapping, as well as simulating the execution of sample programs.  

This project provides practical experience with CPU architecture, instruction sets, and the coordination of core components such as the ALU, register file, instruction and data memory, and control unit. It demonstrates how theoretical concepts in computer organization are applied in designing a functioning CPU model.

## Tools Used

- **Logisim** – for designing the CPU datapath and control unit. 
- **RARS (RISC-V Assembler and Runtime Simulator)** – for testing and simulating assembly programs.

## Features

1. **Custom Instruction Set Design:**
   - Arithmetic Instructions (R-type): `add`, `sub`  
   - Logical Instructions (R-type): `and`  
   - Branch Instructions (B-type): `beq`, `bne`  
   - Load/Store Instructions (I-type, S-type): `lw`, `sw`  
   - Includes mapping of opcode, funct3, and funct7 signals.  

2. **CPU Datapath and Components:**
   - Program Counter (PC) – manages instruction sequence.  
   - ALU – performs arithmetic and logical operations.  
   - Register File – temporary storage for operands and results.  
   - Instruction Memory – stores program instructions.  
   - Data Memory – stores and retrieves data for load/store instructions.  
   - Immediate Generator – extracts immediate values for I-type and B-type instructions.  
   - Control Unit – generates control signals (ALUSrc, RegWrite, MemRead, MemWrite, PCSrc) to coordinate data flow.  

3. **Instruction Execution Plan:**
   - Instruction Fetch (IF)  
   - Instruction Decode (ID)  
   - Execute (EX)  
   - Memory Access (MEM)  
   - Write Back (WB)  

4. **Sample RISC-V Program:**
   - Demonstrates arithmetic operations, memory access, and conditional branching.  
   - Includes commented assembly code illustrating control flow and data handling.

## Installation

No installation is required to view the project. Open the provided **Logisim files** and/or the provided media to explore the CPU design.

## Usage

### CPU Exploration:
- Open the Logisim Evolution project to navigate the CPU datapath.
- Examine components like ALU, register file, instruction memory, data memory, and control signals.
- Use the control signal diagrams to understand instruction execution.

### Running Sample Programs:
- Open the provided RISC-V assembly file in RARS.
- Simulate the program step by step to see arithmetic, logical, load/store, and branch instructions in action.
- Observe how the program interacts with the CPU model components and control signals.

### Instruction Execution:
- Follow the step-by-step execution plan:
  1. Instruction Fetch: PC retrieves instruction from Instruction Memory.
  2. Instruction Decode: Registers read operands, instruction decoded.
  3. Execute: ALU performs operations.
  4. Memory Access: Data Memory read/write for load/store instructions.
  5. Write Back: Results stored in Register File.

### Understanding Control Signals:
- ALUSrc, RegWrite, MemRead, MemWrite, and PCSrc are set according to instruction type.
- Zero signal in ALU determines branching outcomes.
- Immediate Generator produces constants for I-type and B-type instructions.

## Contributing

If you'd like to contribute to this project, please follow these guidelines:

1. Fork the Project  
2. Create your Feature Branch  
3. Commit your Changes  
4. Push to the Branch  
5. Open a Pull Request  

## License

This project is not licensed.

## Acknowledgements

- [Logisim](http://www.cburch.com/logisim/)  
- [RARS (RISC-V Assembler and Runtime Simulator)](https://github.com/TheThirdOne/rars)  
- [W3Schools](https://www.w3schools.com/)
- [Stack Overflow](https://stackoverflow.com/)
- University materials and resources
