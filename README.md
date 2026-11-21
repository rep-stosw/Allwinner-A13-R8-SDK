# Allwinner A13 / R8 BareMetal SDK

![Architecture](https://img.shields.io/badge/Architecture-ARM_Cortex--A8-blue)
![SoC](https://img.shields.io/badge/SoC-Allwinner_A13_R8-orange)
![Language](https://img.shields.io/badge/Language-C_&_Assembly-brightgreen)
![Boot Time](https://img.shields.io/badge/Boot_Time-Sub--Second-red)

**Ultra-fast, high-performance bare-metal framework written completely from scratch in C and Assembly for the Allwinner A13 / R8 SoC (`sun5i` / PocketCHIP).**

Designed for mission-critical embedded applications requiring sub-second boot times, zero OS overhead, and direct hardware register control. Includes custom SPL bootloaders (USB, SD, SPI NOR), hardware-accelerated H.264 Cedar Video Engine, Mali-400 GPU initialization, multi-layer Display Engine, and low-latency digital audio.

## Real Hardware Demonstration

### 1. Mali-400 GPU 3D Hardware Rendering (R8 SoC)

https://github.com/user-attachments/assets/b539e422-f6e2-4604-95e7-118be087c84e

### 2. Mali-400 GPU 3D Hardware Rendering (A13 SoC)

https://github.com/user-attachments/assets/290af72a-0577-41cc-8f61-1dd6e6a5eb95

### 3. JPEG Decoder (13 SoC)

https://github.com/user-attachments/assets/91e4b974-00a9-4b4d-8f50-d4b59a90d865

## The complete SDK includes the following production-ready components:

| Category | Module | Technical Capabilities |
| :--- | :--- | :--- |
| **Bootloaders** | `LoaderUSB` | Custom first-stage USB (FEL) bootloader for direct RAM execution |
| **Bootloaders** | `LoaderSD` | Secure Digital card bootloader (SPL) for MMC media booting |
| **Bootloaders** | `LoaderNOR_SPL` | Ultra-compact SPL optimized for SPI NOR Flash layout |
| **Graphics & Video** | `Mali400(APP)` | Pure bare-metal register initialization for Mali-400 GPU core |
| **Graphics & Video** | `H264(APP)` | Hardware-accelerated video decoding/encoding via Cedar Video Engine |
| **Graphics & Video** | `LCD_Primary(APP)` | Direct Display Engine (DE) control with multi-layer hardware blending |
| **Graphics & Video** | `LCD_Alt(APP)` | Alternative display timing configuration and custom framebuffer layout |
| **Audio & Storage** | `Audio(APP)` | Low-latency digital audio pipeline for internal SoC DAC/ADC |
| **Audio & Storage** | `FatFs(APP)` | High-speed filesystem integration for SD cards and Flash media |
| **Core & System** | `MemTest` | DRAM calibration, cache setup, and stability stress-test utility |
| **Core & System** | `Tiny(APP)` | Minimalist template for core SoC clock/PLL setup and UART debugging |
| **Production** | `H264_Sprites_LRADC_SPI_NOR(APP)` | Combined production firmware running entirely from SPI NOR Flash |
| **Production** | `H264_Sprites_LRADC_SPI_SD_RAM(APP)` | Ultimate system layout with active SD/RAM data caching |

## Need the SDK?
If you require the complete production-ready source code, custom linker scripts, startup codes, and compilation toolchains, please contact the lead architect directly:

> ### **Email: repstosw2018@gmail.com**

*Direct engineer-to-engineer source transfer.*
