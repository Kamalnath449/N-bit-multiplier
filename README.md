# N-Bit Multiplier using Verilog HDL

## Overview

This project implements an **N-Bit Binary Multiplier** using Verilog HDL. The design multiplies two N-bit binary numbers and generates a 2N-bit product output. The project demonstrates fundamental digital design concepts such as combinational logic, arithmetic operations, and hardware description language (HDL) modeling.

## Features

* Parameterized N-bit multiplier design
* Supports multiplication of binary operands of configurable width
* Synthesizable Verilog code
* Easy to simulate and verify
* Suitable for FPGA and ASIC design learning

## Project Structure

```
├── multiplier.v      # N-Bit Multiplier Module
├── testbench.v       # Testbench for simulation
├── waveform.vcd      # Simulation waveform output
└── README.md         # Project documentation
```

## Design Description

The multiplier accepts two N-bit inputs:

* `A` : First operand
* `B` : Second operand

The output is:

* `P` : 2N-bit multiplication result

### Functional Equation

```
P = A × B
```

## Verilog Module Example

```verilog
module multiplier #(parameter N = 4)(
    input  [N-1:0] A,
    input  [N-1:0] B,
    output [2*N-1:0] P
);

assign P = A * B;

endmodule
```

## Simulation

The design can be simulated using:

* EDA Playground
* Icarus Verilog
* ModelSim
* Vivado Simulator

### Example Test Cases

| A  | B  | Product |
| -- | -- | ------- |
| 3  | 2  | 6       |
| 5  | 4  | 20      |
| 7  | 7  | 49      |
| 15 | 15 | 225     |

## Waveform Verification

Simulation waveforms verify that the product output correctly reflects the multiplication of the input operands for all test cases.

## Applications

* Digital Signal Processing (DSP)
* Arithmetic Logic Units (ALU)
* Embedded Systems
* FPGA-based Designs
* VLSI Design and Verification

## Learning Outcomes

Through this project, you will learn:

* Verilog HDL coding
* Combinational circuit design
* Testbench development
* Simulation and waveform analysis
* FPGA/VLSI design fundamentals

