<body>
<img width="1152" height="256" alt="q_logo_refb" src="https://github.com/user-attachments/assets/e415bd7f-e8ac-40d8-8578-0974efcf9b2f" />

<h1 align="center">Quasar Handheld🌠</h1>

### ⚠️Status information 
The project is still under development and it's not made yet, expect software after full hardware development, and the project files, gerbers are outdated! Expect new files tommorow

## ❓ About the device
An advanced, custom-engineered handheld platform utilizing a dual-MCU architecture. The project breaks away from standard single-processor limitations by combining the high-speed wireless capabilities of the ESP32 with the robust, real-time hardware co-processing of an STM32. 

## 🚀 System Architecture & Features
* **Dual-MCU Core:** Features an ESP32 for Wi-Fi/Bluetooth connectivity and main applications, paired with an STM32 co-processor managing low-level hardware routines.
* **Optimized Audio Block:** Integrates an 8-pin digital I2S audio decoder chip, completely replacing bulky legacy analog components (aux jacks, power transistors, protection diodes) with a clean, low-noise digital audio path.
* **Peripherals & I/O:** Complete integration of a display module, dedicated power management/battery circuitry, and high-speed communication lines linking both processors.

## 🛠️ Hardware Stack
* **Main Compute:** ESP32-S3-MINI-1U
* **Co-Processor:** STM32F405RGT6 **Can be accessible via UART or SPI Slave**
* **Audio:** 8 ohm speaker that is managed by D-Class MAX98357A DAC Audio amplifier and Integrated CPT-9019S-SMT-TR Buzzer 
* **PCB Constraints:** 4-Layers, optimized ground plane return paths
* **Power delivery and management:** Uses MAX17260SETD+ Fuel gauge, TP4056 Battery chip charger, AP2112K-3.3 LDO regulator and TPS22917DBVR Load switch.
* **Memory addons:** W25Q128JVS 16kb SPI Flash for secondary firmware and shared APS6404L-SQRx-SN series shared SRAM
* **Haptics and Microphone:** ERM Haptic engine with flyback diode for protection, and MAX9814 Microphone amplifier
* **Display:** TFT SPI ST7789 Colorful Display
* **Gyroscope:** MPU-6050 Chip
* **GPS Navigation:** Ai-Thinker GP-02 GPS module
* **Extension ports:** One USART port 
* **USB Interface:** Uses two receptacle 16 pin USB, one for ESP32 + Charging, second is for STM32 ⚠️**DATA ONLY**
* **Radio things:** Ra-01, NRF24L01, Si4735-D60-GU
* **RFID/NFC:** PN532 with balun transformer (50 ohm coaxial)

* **Note to radio connectors:** I use U.Fl IPEX-1 SMA, and (Hirose SMT-1 Vertical) and also Amphenol 132289 EdgeMount Female SMA connector (use 2.4ghz FPC patches for ESP32-S3-MINI-1U and NRF24l01, 13.56MHZ for RFID and GPRS FPC antenna, or use U.FL to SMA connector, use anything as long if it's 50 ohm connector.)

## 💫 Credits
Thanks to JLCPCB, KiCad i can make this project come true⭐.
And thanks to my teacher that teached the basis of electronics: [Maxym Kaplun](https://github.com/KaplunMaxym).

## 📈 Working on
* Polishing up the board

## ⚖️ Licensing
This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. 

You are welcome to download, study, and modify these design files for personal or educational use. However, **commercial use, mass production, or selling the physical PCBs/assembled units is strictly prohibited** without explicit permission.
</body>

