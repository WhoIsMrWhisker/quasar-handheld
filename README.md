<img width="1066" height="317" alt="q_logo" src="https://github.com/user-attachments/assets/3ea471a5-62e1-420a-bb9b-a05f2a4578e4" />

# Quasar Handheld System
### ⚠️WARNING: The project is still under development and can do a mass changes 
An advanced, custom-engineered handheld platform utilizing a dual-MCU architecture. The project breaks away from standard single-processor limitations by combining the high-speed wireless capabilities of the ESP32 with the robust, real-time hardware co-processing of an STM32. 

To keep fabrication accessible and highly cost-effective, the entire system is routed on a complex **2-layer PCB layout**, navigating high-density routing and digital signals without upgrading to a 4-layer stack.

## 🚀 System Architecture & Features

* **Dual-MCU Core:** Features an ESP32 for Wi-Fi/Bluetooth connectivity and main applications, paired with an STM32 co-processor managing low-level hardware routines.
* **Optimized Audio Block:** Integrates an 8-pin digital I2S audio decoder chip, completely replacing bulky legacy analog components (aux jacks, power transistors, protection diodes) with a clean, low-noise digital audio path.
* **Peripherals & I/O:** Complete integration of a display module, dedicated power management/battery circuitry, and high-speed communication lines linking both processors.
* **Advanced 2-Layer Layout:** Engineered with strict ground plating optimization, stitched copper pours, and carefully placed via-channels to overcome the physical routing constraints of a tight 2-layer grid.

## 🛠️ Hardware Stack
* **Main Compute:** ESP32
* **Co-Processor:** STM32
* **Audio:** Dedicated I2S Digital Audio Decoder and buzzer
* **PCB Constraints:** 2-Layers, optimized ground plane return paths 

## ⚖️ Licensing

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. 

You are welcome to download, study, and modify these design files for personal or educational use. However, **commercial use, mass production, or selling the physical PCBs/assembled units is strictly prohibited** without explicit permission.


