![N|Solid](https://arribada.org/wp-content/uploads/2022/01/arribada_web_logo_g.svg)

# Arribada Argos SMD Module

![Arribada SMD Module Hero Image](https://github.com/arribada/argos-smd-hw/blob/main/Project%20Outputs%20for%20BGA_RF-ArticGR/arribada_smd_hero-1.png)

---

## 🌍 Where to Buy

The **Arribada Argos SMD** module is available for purchase directly from Arribada’s official store:  
👉 [**Buy the Arribada Argos SMD Module**](https://arribada.org/arribada-smd/)

Visit the [Arribada SMD product page](https://arribada.org/arribada-smd/) for up-to-date information, technical documentation, and certification details.

---

## 🛰️ Description

The **Arribada Argos SMD module** is a compact **20x20 mm** PCB designed to act as a **standalone** or **co-processor** module enabling **satellite communication** via the **Kineis network**.

Built around the **STM32WL55** processor and integrated with the **GR5504 power amplifier**, the module provides up to **26 dBm transmission power** and is **pre-certified by CLS**, ensuring immediate deployment for satellite uplink applications.

This repository contains the complete **Altium project** and **production files**.  

The module can be integrated and used across several hardware configurations:

- **Breakout board:** [featherwings-argos-smd-hw](https://github.com/arribada/featherwings-argos-smd-hw) — designed for rapid prototyping with Adafruit Feather nRF52840 or RP2040 boards.  
- **Standalone board:** *Private for now, will be made public soon.*  
- **Linkit-V4-SMD board:** *Not yet opened.*  
- **RSPB board:** *Not yet opened.*

This repository contains the complete **Altium project** and **production files**.  


---

## ⚙️ Configuration

The Argos SMD module requires only **a power supply and an antenna** to operate.

For easy integration and testing, use the [**argos-smd-wings**](https://github.com/arribada/argos-smd-wings) breakout board, which is compatible with **Adafruit Feather nRF52840** or **RP2040** development boards.

### Firmware Resources

- Official Kineis-based firmware:  
  👉 [argos-smd-at-kineis-firmware](https://github.com/arribada/argos-smd-at-kineis-firmware)

- Example STM32 project using AT commands:  
  👉 [SMD_AT_Slave](https://github.com/arribada/SMD_AT_Slave)

---

## 🔌 Pinout

Below is the Argos SMD module pinout:

![Argos SMD Pinout](https://github.com/arribada/argos-smd-hw/blob/main/Project%20Outputs%20for%20BGA_RF-ArticGR/smd_pin_out.png)

---

### System
- **P35:** nRST  
- **P31 / P32:** VDD  
- **P30:** VBAT  

### Power Amplifier
- **P7 / P8:** VDD power amplifier  
- **P9:** LDO enable  
- **P10:** LDO control (GOOD or SEL)  
- **P18:** Antenna output  

### Debug
- **P26:** SWDIO  
- **P25:** SWCLK  
- **P23:** SWDIO  
- **P27:** RF-BUSY  
- **P28:** RF-NRST  

### I2C
- **P33:** SDA  
- **P34:** SCL  

### SPI
- **P24:** NSS  
- **P3:** SPI_SCK  
- **P2:** SPI_MISO  
- **P22:** SPI_MOSI  

### LPUART
- **P4:** UART_RX  
- **P5:** UART_TX  

### UART
- **P11:** UART_RX  
- **P12:** UART_TX  

### Free GPIOs
- **P0:** PB13 (free)  
- **P1:** PB9 (free)

---

## 📘 Device Sheets

- **BGA:** STM32WL55JCI7  
- **STM32WL SMPS configuration** (with STM32WL details sheet)  
- **CLS_1W_3.3V_Lineup configuration** with Guerrilla  

---

## 🧾 Versions

- **V1.0 (2024/05/01):** First release, minor fix (first batch of 150 units)  
- **V0.1d (2023/08/23):** PCB layout under production with H.C.C (4 PCBA to test the design) — 4 layers, HDI board  
- **V0.1 (2023/06/05):** PCB layout finalization and validation phase  

---


## 🔗 Additional Resources

- **Arribada Product Page:** [https://arribada.org/arribada-smd/](https://arribada.org/arribada-smd/)  
- **Firmware:** [argos-smd-at-kineis-firmware](https://github.com/arribada/argos-smd-at-kineis-firmware)  
- **Hardware:** [argos-smd-hw](https://github.com/arribada/argos-smd-hw)  
- **Arduino Testing:** [argos-smd-test-arduino](https://github.com/arribada/argos-smd-test-arduino)  
- **Zephyr Driver (coming soon):** [argos-smd-driver-zephyr](https://github.com/arribada/argos-smd-driver-zephyr)  
- **Hardware Library:** [hardware-lib](https://github.com/arribada/hardware-lib)

---

© Arribada Initiative — Open Hardware for Conservation Technology
