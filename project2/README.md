# Nand2Tetris – Project 2: Boolean Arithmetic

This repository contains my implementation of Project 2: Boolean Arithmetic from the Nand2Tetris course. The goal of this project is to build a set of chips that carry out arithmetic addition, culminating in the construction of the ALU (Arithmetic Logic Unit) of the Hack computer later on.

Building on the logic gates from Project 1, I construct progressively more complex arithmetic components, from a simple Half Adder all the way to a fully functional 16-bit ALU. All chips are implemented using HDL (Hardware Description Language).

---

## Project Overview

Starting from the elementary logic gates built in Project 1, I implement a hierarchy of arithmetic components:

- Adders: HalfAdder, FullAdder, Add16
- Incrementer: Inc16
- Arithmetic Logic Unit: ALU

The ALU is the centerpiece of the Hack computer's CPU. It takes two 16-bit inputs and a set of 6 control bits, and computes one of 18 possible functions, along with two status output bits (`zr` and `ng`).

---

## Project Structure

project2/
├── HalfAdder.hdl
├── FullAdder.hdl
├── Add16.hdl
├── Inc16.hdl
└── ALU.hdl

Note: Each .hdl file is paired with a .tst and .cmp file for testing. The ALU has two test stages: `ALU-basic.tst` (ignoring `zr`/`ng`), and `ALU.tst` for the full implementation

## How To Run

**Online Nand2Tetris IDE (recommended):**
1. Open the simulator at https://nand2tetris.github.io/web-ide/chip/
2. Select Project 2 and the chip you want to test from the drop-down menus.
3. Run the tests and compare output with the `.cmp` file.