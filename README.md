# Allwinner A13 / R8 BareMetal SDK

**Ultra-fast, high-performance bare-metal framework written completely from scratch in C and Assembly for the Allwinner A13 / R8 SoC (`sun5i` / PocketCHIP).**

Designed for mission-critical embedded applications requiring sub-second boot times, zero OS overhead, and direct hardware register control. Includes custom SPL bootloaders (USB, SD, SPI NOR), hardware-accelerated H.264 Cedar Video Engine, Mali-400 GPU initialization, multi-layer Display Engine, and low-latency digital audio.

## Real Hardware Demonstration
* Watch Demo Video 1:
https://github.com/user-attachments/assets/b539e422-f6e2-4604-95e7-118be087c84e

* Watch Demo Video 2:
https://github.com/user-attachments/assets/61212576-08dc-4903-8976-7829025ef200

## Project Directory Structure
![Project Structure](structure.png)

The complete SDK includes the following 13 production-ready components:

1. **MemTest** — DRAM calibration and stability stress-test utility.
2. **LoaderUSB** — Custom first-stage USB bootloader for direct RAM execution.
3. **Tiny(APP)** — Minimalist template for core SoC clock/PLL setup and UART debugging.
4. **Audio(APP)** — Low-latency digital audio pipeline for internal SoC DAC/ADC.
5. **LCD(APP)** — Direct Display Engine (DE) control with multi-layer hardware blending.
6. **LCD(APP)** — Alternative display timing configuration and layout.
7. **FatFs(APP)** — High-speed filesystem integration for SD cards and Flash media.
8. **H264(APP)** — Hardware-accelerated video decoding/encoding via Cedar Video Engine.
9. **LoaderSD** — Secure Digital card bootloader (SPL) for MMC media booting.
10. **H264_Sprites_LRADC_SPI_NOR(APP)** — Combined production firmware running entirely from SPI NOR Flash.
11. **Mali400(APP)** — Pure bare-metal hardware registers initialization for the Mali-400 GPU core.
12. **LoaderNOR_SPL** — Ultra-compact SPL optimized for SPI NOR Flash layout.
13. **H264_Sprites_LRADC_SPI_SD_RAM(APP)** — Ultimate system layout running with active SD/RAM data caching.

## Need the SDK?
If you require the complete production-ready source code, custom linker scripts, startup codes, and compilation toolchains, please contact the lead architect directly:

* **Email:** [repstosw2018@gmail.com]

*Direct engineer-to-engineer source transfer.*
