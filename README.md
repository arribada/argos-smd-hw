![N|Solid](https://arribada.org/wp-content/uploads/2022/01/arribada_web_logo_g.svg)
# Argos SMD module
## Description 

The Argos SMD module is a small PCB (2x2cm) dedicated to act as a standalone or a coprocessor for any new design which required a satelite communication. 
The module is based on STM32WL55 processor and combined with GR5504 power amplifier allowing a comunication up to 26dBm. This module which pass the CLS certification is ready to be used. 

This repository is an altium project with the production files allowed. Please download the hardware-lib repository to have all schematics files used and libraries: https://github.com/arribada/hardware-lib 

## Configuration
The module only required a power supply and an antenna to be ready to be used.

The argos-smd-wings is an example of breakout board ready to be used with Adafruit Feather board nRF52840 or RP2040. Find ressources at the following link : https://github.com/arribada/argos-smd-wings

The firmware based on the Kineis library could be found at : https://github.com/arribada/SMD-AT-Kineis

It is also posible to use the STM32 example for AT command to controle the Sub-Ghz module at this link :
https://github.com/arribada/SMD_AT_Slave

## Pin out
System:
- P35 => nRST
- P31 => VDD
- P32 => VDD
- P30 => VBAT

Power amplifier:
- P7: VDD power amplifier
- P8: VDD power amplifier
- P9: LDO Enable pin
- P10: LDO control pin (GOOD or SEL)
- P18: Antenna out

Debug:
- P26: SWDIO
- P25: SWCLK
- P23: SWDIO
- P27: RF-BUSY
- P28: RF-NRST

I2C:
- P33: SDA
- P34: SCL

SPI:
- P24: NSS
- P3: SPI_SCK
- P2: SPI_MISO
- P22: SPI_MOSI

LPUART:
- P4: UART_RX
- P5: UART_TX

UART:
- P11: UART_RX
- P12: UART_TX

Free: 
- p0: PB13 (free)  
- p1: PB9 (free)

## Device sheet used

- DeviceSheets:
    -   BGA : stm32wl55jci7
	-   STM32WL SMPS configuration with stm32wl details sheet
    -   CLS_1W_3.3V_Lineup configuration with Guerrilla
    


## State
V1.0: (2024/05/01) First release minor fix. => first batch 150 pieces.
V0.1d : (2023/08/23) PCB layout under production with H.C.C (4 PCBA to test the design) => 4xlayers, HDI board 
V0.1 : (2023/06/05) PCB layout finalization and under validation

## Todo
- Create wiki

