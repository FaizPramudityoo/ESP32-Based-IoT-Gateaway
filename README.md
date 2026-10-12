# ESP32-S3 IoT Gateway Hardware

Hardware design files for an ESP32-S3-based IoT gateway, created in Altium Designer. The board brings together network connectivity, industrial interfaces, sensor inputs, local storage, and power regulation in one PCB project.

## Purpose

This project explores a gateway board that can receive data from external sensors or industrial equipment and provide several options for communicating that data to other systems. The repository contains the Altium project, schematics, PCB layout, and related design files.

## Hardware at a Glance

| Section | Components and interfaces |
| --- | --- |
| Main controller | ESP32-S3 |
| Wired network | W5500 Ethernet controller and RJ45 connection |
| Cellular connection | Mini PCIe interface for an EG25-G module |
| Industrial buses | RS-485 and CAN transceiver interfaces |
| Analog inputs | ADS7128, 8-channel ADC over I²C |
| Digital expansion | TCA9534 GPIO expander over I²C |
| Local storage | microSD card interface |
| Power | 5 V input and TPS62132-based 3.3 V regulation |

## Design Files

- `.PrjPcb` — open this file to load the complete project in Altium Designer.
- `.SchDoc` — circuit schematics for the controller and peripheral sections.
- `.PcbDoc` — PCB layout.
- `.PcbStructure` and `.Cam` — supporting board and output configuration files.

The design is organized into separate schematic sheets for functions such as the minimum ESP32 system, power regulation, Ethernet, I²C, SPI, UART, GPIO, and SD card interface.

## Opening the Project

1. Download or clone this repository.
2. Open the `.PrjPcb` file in Altium Designer.
3. Review the schematics and PCB document from the Altium project panel.

## Design Status

This repository contains the hardware design. Electrical behavior, PCB manufacturing results, and operation with connected modules should be confirmed through appropriate review and physical testing before deployment.
