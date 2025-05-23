# Capstone-Project-1

## 📚 Course Information
- **Course:** EE2421 Capstone Project 1  
- **Supervisor:** Bùi Quốc Bảo  
- **Semester:** 242  
- **University:** Ho Chi Minh City University of Technology  

---

## 🧩 Project Description

This project is a Python-based **host programmer tool** for STM32 bootloader communication, designed as part of a capstone project to demonstrate embedded systems integration and serial protocol handling. It is based on the open-source project by [@niekiran](https://github.com/niekiran/BootloaderProjectSTM32) and customized to fit our educational requirements.

The system enables a host PC to communicate with an STM32 board over UART, sending commands such as:

- Retrieve bootloader version and chip ID
- Flash memory erase (sector/mass)
- Memory write using `.bin` files
- Sector protection (read/write)
- Jump to application address

---

## ⚙️ Key Features

- ✅ Command-line interface for sending bootloader commands
- ✅ UART serial communication using `pyserial`
- ✅ CRC32 checksum validation
- ✅ Flash memory control from PC
- ✅ Clear status feedback and debug logs

---

## 🧰 Requirements

- Python 3.7+
- STM32F4 MCU (e.g., STM32F446RE) with a custom bootloader
- USB-to-Serial connection (ST-LINK, USB UART, etc.)
- Firmware binary file (`user_app.bin`)
- Windows or Linux environment

Install dependencies:

```bash
pip install pyserial
