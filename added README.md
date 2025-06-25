# 🔧 Custom Von Neumann CPU Architecture

A complete 8-bit CPU implementation built in Logisim, demonstrating fundamental processor architecture principles through hands-on simulation.

---

## 📋 Overview

This project implements a custom Central Processing Unit (CPU) based on the Von Neumann architecture, developed as part of the EEEG202 course at Kathmandu University. The CPU features a complete instruction cycle (fetch-decode-execute) using fundamental digital logic components, providing deep insights into how processors work at the hardware level.

---

## 🏗️ Architecture

The CPU follows the Von Neumann architecture model with shared memory for both instructions and data, implementing a full instruction processing pipeline from basic building blocks.

---

## 🔍 Components

### 🧠 Core Processing Units
- 🧮 **8-bit Arithmetic Logic Unit (ALU)** — Performs basic addition operations
- 📥 **Accumulator Registers A & B** — Hold input values for ALU operations
- 📤 **Output Register** — Stores final computation results

### 🗃️ Memory Management
- 📦 **Memory Buffer Register (MBR)** — Handles data transfer to/from memory
- 📦 **Memory Address Register (MAR)** — Manages memory addressing
- 🧱 **RAM Module** — Organized memory with distinct sections:
  - Instruction Memory: Addresses `0–7`
  - Data Memory: Addresses `8–15`

### ⚙️ Control & Execution
- ⏱️ **Program Counter (PC)** — Directs instruction execution flow
- 🔍 **Instruction Register (IR)** — Decodes binary opcodes into control signals
- 🧩 **Control Unit (CU)** — Manages operation sequencing through micro-operations

### 🔄 Data Communication
- 🔄 **Internal Bus** — Facilitates data communication between processor components
- 🔄 **External Bus** — Handles data transfer between processor and RAM

---

## 📌 Instruction Set

The CPU supports four fundamental instructions:

| Opcode | Binary | Operation              |
|--------|--------|------------------------|
| 0000   | `0000` | Load to Register A     |
| 0001   | `0001` | Load to Register B     |
| 0010   | `0010` | Add (A + B)            |
| 0011   | `0011` | Store Result           |

---

## 🔄 Instruction Cycle

Each instruction follows the standard fetch-decode-execute cycle:

1. **Fetch**: Program Counter addresses instruction memory, instruction loaded into IR  
2. **Decode**: Control Unit interprets opcode and generates control signals  
3. **Execute**: ALU performs operation, results stored in appropriate registers

---

## 💡 Advanced Features

### 🔁 Looping Logic
Despite the minimal instruction set, the CPU demonstrates complex behavior through careful instruction sequencing, enabling:
- Repeated operations
- Sequential data processing
- Basic program flow control

### 🧭 Memory Organization
- Harvard-inspired memory layout (separate sections within shared RAM)
- Efficient use of 16-address space
- Direct memory access using MAR/MBR register pair

---

## 🛠️ Technology Stack

- 🧪 **Simulation Tool**: Logisim
- 🧱 **Architecture**: Von Neumann
- 📐 **Data Width**: 8-bit
- 💾 **Memory**: 16 addresses (8 instruction + 8 data)

---

## 🚀 Getting Started

### ✅ Prerequisites
- Logisim installed
- Basic knowledge of digital logic and computer architecture

### ▶️ Running the Simulation
1. Clone this repository  
2. Open the `.circ` file in Logisim  
3. Use simulation controls to step through each instruction  
4. Monitor register values and memory content live

---

## 📊 Technical Specifications

- **Word Size**: 8 bits  
- **Memory Capacity**: 16 addresses  
- **Instruction Format**: 4-bit opcode  
- **Clock Cycle**: Manual/controlled stepping  
- **Bus Architecture**: Separate internal and external buses

---

## 🎯 Learning Outcomes

Gain hands-on experience with:
- ✅ Processor design fundamentals
- ✅ Digital logic implementation
- ✅ Memory organization and addressing
- ✅ Control flow using opcode sequencing
- ✅ Internal and external bus architecture

---

## 🔗 Applications

This project is ideal for:
- 🏫 Computer architecture education
- 🔧 Digital systems design
- 🧪 Processor simulation/testing
- 🤖 Hardware-software interface learning

---

## 📚 Educational Context

Developed for the EEEG202 course at Kathmandu University (Electrical Systems Design), this project bridges electrical and computer engineering by demonstrating how low-level hardware logic enables meaningful computation.

---

## 🤝 Contributing

Feel free to fork this project and experiment with:
- 🧮 Additional instruction types
- 🗂️ Extended memory or RAM modules
- 🧠 More advanced ALU operations
- 🧩 Custom control logic enhancements

---

## 📄 License

This project is open-source and free for educational use.

---

*This project demonstrates that even with a minimal instruction set, complex computational behavior is achievable through thoughtful hardware design and sequencing — a testament to the elegance of fundamental computer architecture principles.*
