# 🧮 Basic Calculator - x8086 Assembly

This project is a simple **calculator written in x8086 Assembly language** that performs basic arithmetic operations such as **Addition, Subtraction, Multiplication, and Division**.

---

## 🚀 Features

- ✅ Addition
- ✅ Subtraction
- ✅ Multiplication
- ✅ Division
- ✅ User-friendly input/output via interrupts
- ✅ Modular design using subroutines
- ✅ ASCII to numeric input conversion

---

## 📋 How It Works

### 1. **User Interface**
- The program prompts the user to select an arithmetic operation:
  - **Add**
  - **Subtract**
  - **Multiply**
  - **Divide**

### 2. **Input Handling**
- Accepts input from the user for both operands.
- Converts ASCII characters to numeric format using subroutines.

### 3. **Arithmetic Operations**
- Performs the selected operation using registers and instructions.
- Stores the result appropriately.

### 4. **Output Display**
- Converts result back to ASCII.
- Displays it to the screen.
- Waits for any key to exit.

---

## 🧠 Concepts Covered

This project is ideal for beginners learning x86 assembly. It demonstrates:

- 🗃️ Register and memory usage  
- 📥 Handling user input and output via `INT 21h`  
- ➕ Arithmetic instruction handling  
- ♻️ Subroutine usage for clean and modular code  

---

## 📦 Requirements

- DOSBox or any x86 emulator  
- TASM/MASM Assembler  

---

## 📂 File Structure

```plaintext
Basic-Calculator/
├── calculator.asm       # Main source code
├── README.md            # Project documentation (this file)
