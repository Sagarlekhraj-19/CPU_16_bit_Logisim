# 16-Bit CPU Implementation

A complete 16-bit CPU implementation in Logisim, developed as part of the Introduction to Computational Thinking course at IBA Karachi, Fall '24.

## Overview

This project implements a custom 16-bit CPU architecture with support for arithmetic, logical, memory, and control operations. The CPU is built using modular components and can execute programs written in BOSS Script assembly language.

## Core Components

- **MBR** (Memory Buffer Register) - Holds data being transferred to/from memory
- **MAR** (Memory Address Register) - Stores memory addresses for read/write operations
- **RAM** - Random Access Memory for data storage
- **ROM** - Read Only Memory for program instructions
- **CPU** - Central Processing Unit for instruction execution
- **ALU** - Arithmetic Logic Unit for computations
- **PC** (Program Counter) - Tracks the current instruction address
- **Control Lines** - Signal pathways for coordinating operations

## Instruction Set

### Arithmetic & Logic Operations
| Opcode | Instruction | Description |
|--------|-------------|-------------|
| 0000 | Multiply | Multiply two values |
| 0001 | Compare | Compare two values |
| 0010 | Add | Addition operation |
| 0011 | Sub | Subtraction operation |
| 0100 | Logical OR | Bitwise OR |
| 0101 | Logical AND | Bitwise AND |
| 0110 | Logical XOR | Bitwise XOR |
| 0111 | Logical NOT | Bitwise NOT |

### Memory & Special Operations
| Opcode | Instruction | Description |
|--------|-------------|-------------|
| 1000 | MATMULT 2X2 | Matrix multiplication (2x2) |
| 1010 | STO | Store to memory |
| 1011 | STO Overflow | Store with overflow handling |
| 1100 | MOVE MEM | Move memory contents |
| 1101 | SWAP MEM | Swap memory locations |
| 1110 | SWAP REG | Swap register contents |

## Project Files

- **final_viva_cpu.circ** - Main CPU circuit design
- **BOSS_SCRIPT_A** - Assembly program example A
- **BOSS_SCRIPT_B** - Assembly program example B
- **BOSS_SCRIPT_INST** - Instruction set reference
- **truth_table.xlsx** - Truth tables for logic operations

## Usage

1. Open `final_viva_cpu.circ` in Logisim
2. Load a BOSS Script program into ROM
3. Run the simulation to execute instructions
4. Monitor registers and memory to observe program execution

## Architecture Highlights

- 16-bit data path
- Modular design with reusable components (adders, multipliers, comparators)
- Support for both register and memory operations
- Instruction decoder and control unit for orchestrating operations
- Built-in overflow detection for arithmetic operations

---

*Developed at IBA Karachi | Introduction to Computational Thinking, Fall 2024*
