# Capstone-Project-1

## 📚 Course Information
- **Course:** EE2421 Capstone Project 1  
- **Supervisor:** Bùi Quốc Bảo  
- **Semester:** 242  
- **University:** Ho Chi Minh City University of Technology  

---

## 🧩 Project Description

This project is a Python-based **host programmer tool** for STM32 microcontrollers, designed to communicate with a custom bootloader over UART. It enables the user to:

- Upload firmware (`.bin` file)
- Erase flash memory (sector or mass erase)
- Write to memory addresses
- Manage read/write protection for flash sectors
- Retrieve microcontroller details like chip ID, bootloader version, RDP level

It serves as a learning platform to understand:
- Low-level embedded systems communication
- Serial protocols
- Bootloader architecture on STM32

---

## ⚙️ Features

- UART Serial Communication using `pyserial`
- CRC32-based data integrity check
- Command structure with length, payload, and CRC
- Interactive command-line interface for issuing commands
- Support for multiple STM32 bootloader commands

---

## 🧰 Requirements

- Python 3.7+
- STM32F4 (e.g., STM32F446RE) with custom bootloader flashed
- USB-to-Serial connection (e.g., via ST-LINK or USB TTL)
- A `.bin` firmware file (`user_app.bin`)

### Python dependencies:

```bash
pip install pyserial
