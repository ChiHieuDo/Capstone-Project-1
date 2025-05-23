# Capstone-Project-1

## 📚 Course Information
- **Course:** EE2421 Capstone Project 1  
- **Supervisor:** Bùi Quốc Bảo  
- **Semester:** 242  
- **University:** Ho Chi Minh City University of Technology  

---

## 🧩 Project Overview

This project is my individual submission for the EE2421 Capstone Project. It demonstrates how to communicate with an STM32 microcontroller bootloader over UART using Python.

The implementation is **entirely based on the open-source project by [@niekiran](https://github.com/niekiran/BootloaderProjectSTM32)**. I have not modified the original code. My goal was to understand and apply the existing system to my STM32F4 development board for testing and learning purposes.

---

## 💻 What This Project Does

Using the provided Python script and STM32 bootloader firmware, you can:

- Read bootloader version, chip ID, and RDP status
- Perform flash erase and memory writes
- Enable/disable flash protection
- Jump to user application code

---

## 📦 Files Used

- `STM32_Programmer_V1.py`: Python host tool (used without modification)
- STM32 bootloader C code: Built and flashed using Keil (from original repo)
- `user_app.bin`: Test firmware (provided separately)

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


## 🙏 Credits

This project is fully credited to [@niekiran](https://github.com/niekiran) and his repository [BootloaderProjectSTM32](https://github.com/niekiran/BootloaderProjectSTM32).  
I only used it for academic and educational purposes.

---

## 📜 License

Used under [the original repository’s terms](https://github.com/niekiran/BootloaderProjectSTM32). This version is for educational purposes only.

## Install dependencies:

```bash
pip install pyserial
