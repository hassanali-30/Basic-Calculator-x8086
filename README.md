# x8086 Assembly Calculator

A menu-driven calculator written in 8086 Assembly for the DOS environment. The program accepts keyboard input and performs addition, subtraction, multiplication, and division using low-level registers, arithmetic instructions, reusable subroutines, and DOS interrupts.

This project is a compact example of how a command-line application works close to the hardware level, including character input, ASCII-to-number conversion, arithmetic processing, and numeric result display.

## Features

- Addition, subtraction, multiplication, and division
- Interactive menu and keyboard input
- ASCII digit to numeric-value conversion
- Numeric result to displayable ASCII conversion
- Reusable input and output subroutines
- DOS keyboard and console services through `INT 16h` and `INT 21h`
- 16-bit register-based arithmetic

## How It Works

1. The program displays an operation menu.
2. The user selects an arithmetic operation.
3. Numbers are read one character at a time from the keyboard.
4. The input subroutine converts ASCII digits into a numeric value.
5. The selected arithmetic instruction processes the values.
6. The output subroutine converts the result into displayable digits.
7. The result is printed through DOS console services.

## Requirements

- DOSBox or another compatible x86/DOS emulator
- TASM or MASM assembler
- TLINK or the linker included with the selected assembler

This is a real-mode DOS application. It is not a native Linux or modern Windows executable.

## Running the Program

Place `calculator.asm` in a directory available inside DOSBox, then assemble and link it with the installed toolchain.

Example TASM workflow:

```dos
tasm calculator.asm
tlink calculator.obj
calculator.exe
```

The exact commands may differ between TASM, MASM, and their linker versions.

## Project Structure

```text
calculator.asm   # 8086 Assembly source code
README.md        # Project documentation
License          # License information
```

## Concepts Demonstrated

- 8086 registers and arithmetic instructions
- DOS interrupt services
- Keyboard input and console output
- Subroutine calls and stack usage
- ASCII and numeric conversion
- Conditional jumps and program control flow

## Limitations

- Designed for simple positive integer input.
- Arithmetic uses 16-bit registers and may overflow for large values.
- Division-by-zero validation should be added before production use.
- The program requires a DOS-compatible emulator and assembler toolchain.
