<img width="212" height="133" alt="q_logo (1)" src="https://github.com/user-attachments/assets/ecb84f02-4001-4c3c-8e0b-73e249a3dcd5" />

# Quasar Handheld
### ⚠️STATUS WARNING: The project is still under development and it's not made yet, expect software after full hardware development
An advanced, custom-engineered handheld platform utilizing a dual-MCU architecture. The project breaks away from standard single-processor limitations by combining the high-speed wireless capabilities of the ESP32 with the robust, real-time hardware co-processing of an STM32. 
To keep fabrication accessible and highly cost-effective, the entire system is routed on a complex **2-layer PCB layout**, navigating high-density routing and digital signals without upgrading to a 4-layer stack.

## 🚀 System Architecture & Features
* **Dual-MCU Core:** Features an ESP32 for Wi-Fi/Bluetooth connectivity and main applications, paired with an STM32 co-processor managing low-level hardware routines.
* **Optimized Audio Block:** Integrates an 8-pin digital I2S audio decoder chip, completely replacing bulky legacy analog components (aux jacks, power transistors, protection diodes) with a clean, low-noise digital audio path.
* **Peripherals & I/O:** Complete integration of a display module, dedicated power management/battery circuitry, and high-speed communication lines linking both processors.
* **Advanced 2-Layer Layout:** Engineered with strict ground plating optimization, stitched copper pours, and carefully placed via-channels to overcome the physical routing constraints of a tight 2-layer grid.

## 🛠️ Hardware Stack
* **Main Compute:** ESP32-S3-MINI-1U
* **Co-Processor:** STM32F405RGT6 **Can be accessible via UART or SPI Slave**
* **Audio:** 8 ohm speaker that is managed by D-Class MAX98357A DAC Audio amplifier and Integrated CPT-9019S-SMT-TR Buzzer 
* **PCB Constraints:** 2-Layers, optimized ground plane return paths
* **Power delivery and management:** Uses MAX17260SETD+ Fuel gauge, MCP73831-2-MC Battery charger, AP2112K-3.3 LDO regulator and TPS22917DBVR Load switch.
* **Memory addons:** W25Q128JVS 16kb SPI Flash for secondary firmware and shared APS6404L-SQRx-SN series shared SRAM
* **Haptics and Microphone:** ERM Haptic engine with flyback diode for protection, and MAX9814 Microphone amplifier
* **Display:** TFT SPI ST7789 Colorful Display
* **Gyroscope:** MPU-6050 Chip
* **GPS Navigation:** Quectel_L80-R GPS module
* **Software Defined Radio:** Si4735-D60-GU
* **Extension ports:** Two SPI ports, One I2C and one USART port **STM32 ONLY**
* **USB Interface:** Uses two receptacle 16 pin USB, one for ESP32 + Charging, second is for STM32 ⚠️**DATA ONLY**

## 💫 Credits
Thanks to JLCPCB, KiCad i can make this project come true⭐.
And thanks to my teacher that teached the basis of electronics: [Maxym Kaplun](https://github.com/KaplunMaxym).

## 📈 Working on
* Transfering NRF Breakout module on pcb

## ⚖️ Licensing
This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. 

You are welcome to download, study, and modify these design files for personal or educational use. However, **commercial use, mass production, or selling the physical PCBs/assembled units is strictly prohibited** without explicit permission.


