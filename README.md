# Cyberpunk Nexus — ESP32-P4 LVGL UI Boilerplate

![Cyberpunk Nexus visual theme artwork](Splash%20BoilerPlate_ESP32-P4-WIFI6-Touch-LCD-7B_1024x600_Cyberpunk_Nexus.png)

*Cyberpunk Nexus theme artwork showing this project's visual direction. It is not a photograph of physical hardware or a running-device screenshot.*

Cyberpunk Nexus is a native C / ESP-IDF embedded UI boilerplate and public reference for the Waveshare ESP32-P4-WIFI6-Touch-LCD-7B. It preserves a documented, hardware-proven ESP32-P4 and LVGL 9 baseline with the Cyberpunk Nexus HMI theme.

This repository provides an earlier-generation ForgeUI reference for a 1024×600 touchscreen HMI on the Waveshare ESP32-P4-WIFI6-Touch-LCD-7B, using ESP-IDF, LVGL 9, and the Cyberpunk Nexus visual theme.

## ForgeUI Ecosystem

ForgeUI is developed by [RTechAI](https://github.com/RTechAI).

The [ForgeUI website](https://forgeui.co.nz) is the official home of the ForgeUI embedded UI/HMI development ecosystem.

ForgeUI Studio is the current visual embedded UI/HMI development environment for supported ESP32 hardware.

[ForgeUI Hosted Studio](https://studio.forgeui.co.nz) is the hosted, browser-based ForgeUI Studio application and is available for public registration.

RTechAI's GitHub organization hosts ForgeUI public repositories, hardware references, framework baselines, examples, and related open development work.

This repository is an earlier ESP32-P4 ForgeUI reference created during the ESP32-P4 UI Studio / ForgeUI One era. It remains a public technical reference and is not represented as source or generated output from current ForgeUI Hosted Studio.

## Overview

The project provides a concise starting point for embedded touchscreen UI work on the documented Waveshare target. It combines an ESP-IDF project, LVGL UI runtime, display and touch integration, and a single-page HMI structure.

## Hardware Target

Validated on the documented baseline:

- Waveshare ESP32-P4-WIFI6-Touch-LCD-7B
- ESP32-P4
- 7-inch, 1024×600 display
- EK79007 MIPI DSI display controller
- GT911 capacitive touch
- Waveshare ESP32-P4-WIFI6-Touch-LCD-7B BSP

## Software Stack

| Layer | Baseline |
| --- | --- |
| Firmware | Native C with ESP-IDF 5.5.4 |
| UI | LVGL 9.2.2 |
| Target | `esp32p4` |
| Display and touch | Waveshare BSP, EK79007, GT911 |

## What This Project Demonstrates

- An ESP32-P4 LVGL 9 embedded UI/HMI baseline
- MIPI DSI display and GT911 touch integration for the documented board
- A single-page Cyberpunk Nexus UI/theme direction
- A modular ForgeUI One-era project layout with display, touch, audio, Wi-Fi, RTC, and SD support sources

## UI / Theme

The local hero image is Cyberpunk Nexus visual/theme artwork. It communicates the intended HMI aesthetic only; it does not establish physical hardware configuration or device validation.

## Hardware and Runtime Baseline

This repository retains the ForgeUI One runtime/reference baseline used by this historical project generation. Its source and configuration document the ESP32-P4 target, Waveshare board integration, LVGL 9.2.2 dependency, and ESP-IDF 5.5.4 lockfile baseline.

## Project Structure

```text
.
├── main/                         # Application, ForgeUI One-era runtime, and UI assets
│   ├── main.c                    # ESP-IDF application entry point
│   ├── 01_FG_Runtime.*           # Runtime integration
│   ├── 20_RTC.*                  # RTC support
│   ├── 30_WIFI.*                 # Wi-Fi support
│   ├── 40_SIDEBAR.*              # Sidebar UI
│   ├── 40_SD.*                   # SD-card support
│   ├── 90_Studio_Export.*        # Historical Studio UI export integration
│   └── assets/                   # Theme, icon, and generated asset sources
├── components/bsp_extra/         # Board-specific BSP extension
├── docs/                         # Setup notes, architecture, and visual assets
├── dependencies.lock             # Resolved ESP-IDF component baseline
├── sdkconfig.defaults            # ESP32-P4 default configuration
└── CMakeLists.txt                # ESP-IDF project root
```

## Build and Flash

Install and activate an ESP-IDF 5.5.4 environment, then run from the repository root:

```bash
idf.py set-target esp32p4
idf.py build
idf.py flash monitor
```

Choose the appropriate serial port for your system if the ESP-IDF environment does not select one automatically.

## Historical ForgeUI Context

Cyberpunk Nexus was visually designed and exported using the historical [ESP32-P4 UI Studio](https://github.com/RTechAI/esp32p4-ui-studio), then integrated with the [ForgeUI One](https://github.com/RTechAI/ForgeUI-One) runtime/reference baseline. Those earlier projects describe this repository's lineage; they are distinct from the current ForgeUI Studio environment and ForgeUI Hosted Studio application.

## Current ForgeUI Studio

The [ForgeUI website](https://forgeui.co.nz) is the official home of the ForgeUI embedded UI/HMI development ecosystem. [ForgeUI Hosted Studio](https://studio.forgeui.co.nz) is the hosted browser-based ForgeUI Studio application.

ForgeUI Studio is the current visual embedded UI/HMI development environment for supported ESP32 hardware.

ForgeUI Hosted Studio is available for public registration.

## Related ForgeUI Projects

- [ForgeUI One](https://github.com/RTechAI/ForgeUI-One) — the historical runtime/reference baseline for this project generation
- [ForgeUI P4](https://github.com/RTechAI/ForgeUI-P4) — related ESP32-P4 ForgeUI work
- [ESP32-P4 LVGL Boilerplate 3](https://github.com/RTechAI/ESP32-P4-LVGL-Boilerplate-3) — related ESP32-P4/LVGL reference work
- [ESP32-P4 UI Studio](https://github.com/RTechAI/esp32p4-ui-studio) — the historical local Studio repository

## About ForgeUI

[ForgeUI](https://forgeui.co.nz) is developed by [RTechAI](https://github.com/RTechAI).

ForgeUI Studio is the current visual embedded UI/HMI development environment for supported ESP32 hardware.

[ForgeUI Hosted Studio](https://studio.forgeui.co.nz) is the hosted, browser-based ForgeUI Studio application and is available for public registration.

RTechAI is the GitHub home for ForgeUI public repositories, hardware references, framework baselines, and example projects.

## License and Third-Party Software

This project is licensed under the repository's [ForgeUI Source Available License](LICENSE). See [THIRD_PARTY_LICENSES.md](THIRD_PARTY_LICENSES.md) for notices covering integrated third-party software.

## Support

Questions, feature requests, and bug reports are welcome. Contact: forgeui.esp32@gmail.com.
