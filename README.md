# 📟 Intel 8086 Microsystem Design & Peripheral Interfacing

A comprehensive hardware-software co-design project featuring a custom microcomputer system based on the **Intel 8086** architecture. This project involves complex memory mapping, address decoding, and the development of low-level drivers in **8086 Assembly**.

## 🏗️ System Architecture

The microsystem is engineered with a modular memory and I/O structure, utilizing specific industrial-grade components:

### 💾 Memory Configuration
* **128 KB EPROM:** Implemented using **27C2048** circuits.
* **64 KB SRAM:** Implemented using **62512** circuits.

### 🔌 Peripheral Interfacing & Addressing
The system features dynamic address decoding controlled by hardware microswitches (S1, S2):
* **8251 USART (Serial Interface):** 
* **8255 PPI (Parallel Interface):** 
* **User Interface:** 6-digit 7-Segment Display, 6 Status LEDs, and a 12-key Matrix Mini-Keyboard.

## 💻 Software Development (8086 Assembly)

The software layer consists of a modular library of subroutines designed for low-level device control and I/O operations.

### Key Subroutines Implemented:
* **Device Initialization:** Hardware-level programming for the **8251 USART** and **8255 PPI** controllers.
* **Serial Communication:** Robust routines for character transmission and reception.
* **Parallel I/O:** Specialized routine for character emission via the 8255 interface.
* **User Input Handling:** A scanning routine for the 12-contact matrix mini-keyboard.
* **Visual Feedback:**
    * LED control (ON/OFF) routines for status monitoring.
    * Hexadecimal character display routine for the 6-digit 7-segment module.

## 🛠️ Hardware Design Logic
The project demonstrates advanced concepts in computer architecture:
* **Address Decoding:** Logic gates and decoders configured to handle overlapping memory and I/O maps.
* **Bus Management:** Proper synchronization of Data, Address, and Control buses for the 8086 CPU.
* **Switch-Based Configuration:** Real-time memory map adjustment via physical microswitches.


---
*Developed as a technical project focusing on low-level hardware-software integration and microprocessor-based system design.*
