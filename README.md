# About
------------------
This project is a comnputer simulation which uses logisim to simulate a working processor and other I/O devices 

This was implemented by Zohaib and Ying.
This is version 1.0 of the project.

# Getting Started!
------------------
Use the assemble.exe to convert mips code into binary. 
To execute the code in the command line you must follow the following format:
"./assemble input.asm output.bin"

# Project Design
------------------
## Processor

![ALT text](Assets/Processor.png)

The processor consists of the control, ALU, and instant-memory. It has both input from and output to the bus, which is connecrted to other I/O devices, such as keyboard and monitor. 

### Regfile
The regfile circuit contains 32 32 bits MIPS registers. It takes in rd, rd select, rs select, rt select, and write enable. The circuit outputs rt and rs values. Rd is the input data value to the regfile and rd select is the register on which to store the data value when write enable is 1. Similarly, rt and rs are data output values, and rt-select an rs-select are the registers from which to retrieve data from

### control

![picture of the control circuit](Assets/Control.png)
