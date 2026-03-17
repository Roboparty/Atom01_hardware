# ROBOTO

**[中文](./README_cn.md)** | English

> **Project Introduction:** This project is an open-source bipedal robot. It aims to lower the assembly threshold by providing a "nanny-level" assembly tutorial from mechanical structure to circuit connection.

---

## 📚 Core Documentation Navigation

We have prepared detailed PDF manuals for beginners. **Please be sure to read them in the following order:**

| Order | Document Name | Description | Location |
| :---: | :--- | :--- | :--- |
| 1️⃣ | **[Installation Manual-0317.pdf](00_Docs/安装手册-0317.pdf)** | Core assembly tutorial | `00_Docs/` |
| 2️⃣ | **[Roboto_origin Wiring Guide.pdf](00_Docs/Roboto_origin走线说明.pdf)** | Electronic wiring guide | `00_Docs/` |
| 3️⃣ | **[Pin Calibration Guide.pdf](00_Docs/插销标定说明.pdf)** | Pin calibration method | `00_Docs/` |
| 4️⃣ | **[3D Printed Parts Calibration Guide.pptx](00_Docs/3D打印件标定说明.pptx)** | 3D printing calibration guide | `00_Docs/` |

---

## 📂 Project File Structure

This repository uses a modular structure, organized as follows:

```text
├── 00_Docs/                         # [Docs] Core manuals and lists
│   ├── 3D打印件标定说明.pptx        # 3D Printing Calibration Guide
│   ├── 安装手册-0317.pdf             # Installation Manual
│   ├── 插销标定说明.pdf              # Pin Calibration Guide
│   ├── Roboto头原型机 (RoboParty Roboto Origin) 散件清单 V1.1.3.xlsx # Parts List
│   ├── Original-0310.pdf             # Original Document
│   ├── Roboto_origin走线说明.pdf     # Wiring Guide
│
├── 01_SW_Project/                   # [Source] SolidWorks engineering files
│   └── robo_origin_2.0               # Roboto Origin 2.0 SW Project
│
├── 02_Manufacturing/                # [Manufacturing] Production files
│   ├── 3D_Printing                  # 3D Printing related files
│   └── CNC_Machining                # CNC Machining related files
│
└── 03_URDF/                         # [Simulation] Robot Description Files
    ├── meshes                       # Simulation model mesh files
    ├── urdf                         # URDF configuration files
    ├── Readme.md                    # URDF folder Readme
    └── robo_origin.png              # Image file