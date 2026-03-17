# RBE_Board V2.0 - Robotic Electrical Hub

**[中文](./README_cn.md)** | English

![Manufacturer](https://img.shields.io/badge/Manufacturer-RoboParty-blue)
![Hardware](https://img.shields.io/badge/Hardware-V2.0-green)
![OS](https://img.shields.io/badge/OS-Linux_Only-orange)

> **Project Introduction:** The **RBE_Board V2.0** is an integrated circuit board designed by **RoboParty** for high-performance bipedal robots. It integrates three key functions: **48V-to-5V step-down conversion**, **power distribution**, and **USB-to-CAN communication**. This board acts as the "electrical hub" of the robot, responsible for power allocation and communication signal distribution.

---

## 📖 Specifications

As the key connection between the battery, the main control board (e.g., Orange Pi 5 Plus), and the limb actuators, the core specifications are as follows:

### 1. Hardware Specifications Table

| Parameter Category | Specification | Notes |
| :--- | :--- | :--- |
| **Power Input** | XT60 Terminal, 48VDC | Connect to Battery PACK |
| **5V Output** | Type-C Interface, Max 8A | Power supply for Main Control Board (e.g., Orange Pi 5 Plus) |
| **48V Output** | XT30 (2+2) Terminals × 4 | Distributed to limb motors |
| **Communication Interface** | USB 2.0 (Type-C) | Connects to Main Control Board for USB-to-CAN function |
| **Cooling Supply** | GH1.25 Interface, 5V | Powers system fans |
| **Dimensions** | 80mm × 60mm | Compact design |

---

## 📂 Repository Structure

This repository contains all engineering files required for manufacturing and utilizing this module:

```text
├── 00_Docs/                         # Documentation
│   ├── Images/                      # Interface & Render Images
│   │   ├── RBE_Board_v2.0_interface_bottom.PNG  # Bottom Interface Definition
│   │   ├── RBE_Board_v2.0_interface_top.PNG     # Top Interface Definition
│   │   └── RBE_Board_v2.0_render.JPEG           # 3D Render Image
│   ├── 3D_PCB5_11_2026-2-1.step    # 3D Structure Model File
│   └── 三合一电路V1.0硬件说明.pdf   # Detailed Hardware Design Principles (Chinese)
│
├── 01_Gerber/                       # PCB Manufacturing Files
│   └── Gerber_RBE_Board_v2.0.zip    # Gerber File Archive
│
├── 02_Assembly/                     # Assembly Files
│   ├── BOM_RBE_Board_v2.0.xlsx      # Bill of Materials (BOM)
│   └── PickAndPlace_RBE_Board_v2.0.xlsx # Pick and Place Coordinates
│
├── README.md                        # English Readme
└── README_cn.md                     # Chinese Readme