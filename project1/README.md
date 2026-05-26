Nand2Tetris – Project 1: Elementary Logic Gates

This repository contains my implementation of Project 1: Elementary Logic Gates from the Nand2Tetris course. The goal of this project is to build a set of basic logic gates and combinational chips using only a single primitive gate: NAND.

From this single building block, I construct all fundamental components needed for a computer system, including multiplexers, demultiplexers, and bitwise logic gates.  All chips are implemented using HDL(Hardware Description Language).



******Project Overview********

Starting from a single primitive gate (Nand), I implement a hierarchy of logic components:

Basic logic gates: Not, And, Or, Xor
Multiplexers & demultiplexers: Mux, DMux
16-bit variants: Not16, And16, Or16, Mux16
Multi-way logic chips:
Or8Way
Mux4Way16
Mux8Way16
DMux4Way
DMux8Way

These components form the foundational building blocks for the CPU and memory systems in later Nand2Tetris projects.

****Project Structure****
projects/01/
├── Nand.hdl        (provided)
├── Not.hdl
├── And.hdl
├── Or.hdl
├── Xor.hdl
├── Mux.hdl
├── DMux.hdl
├── Not16.hdl
├── And16.hdl
├── Or16.hdl
├── Mux16.hdl
├── Or8Way.hdl
├── Mux4Way16.hdl
├── Mux8Way16.hdl
├── DMux4Way.hdl
└── DMux8Way.hdl

Note: Each .hdl file is paired with a .tst and .cmp file for testing

***HOW TO RUN***
Online Nand2Tetris IDE:
1. Open chip in provided simulator.
https://nand2tetris.github.io/web-ide/chip/
2. Run tests and compare output with .cmp file.
