# x8086 Assembly Calculator

A menu-driven calculator written in x8086 Assembly. It supports addition, subtraction, multiplication, and division while demonstrating low-level input, output, arithmetic, and subroutine design.

## Features

- Addition, subtraction, multiplication, and division
- ASCII-to-number conversion for user input
- Result conversion back to displayable text
- Console interaction through DOS interrupts
- Reusable subroutines for input, calculation, and output

## Requirements

- DOSBox or another x86-compatible emulator
- TASM or MASM assembler

## Run

1. Open the project in DOSBox.
2. Assemble `calculator.asm` with TASM or MASM.
3. Link the generated object file.
4. Run the resulting executable.

The exact assembler and linker commands depend on the installed toolchain.

## Project Structure

```text
calculator.asm   # Main Assembly source
README.md        # Project documentation
License          # License information
```

## Concepts Demonstrated

- x86 registers and memory
- Arithmetic instructions
- DOS `INT 21h` input/output
- Subroutines and control flow
- Character and numeric conversion