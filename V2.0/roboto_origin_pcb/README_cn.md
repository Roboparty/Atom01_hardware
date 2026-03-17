# RBE_Board V2.0 - 机器人电气核心枢纽

**[中文](./README_cn.md)** | [English](./README.md)

!<Manufacturer>
!<Hardware>
!<OS>

> **项目简介：** RBE_Board V2.0 是萝博派对 (RoboParty) 专为高性能双足机器人设计的集成化电路板。该板卡将 **48V转5V降压模块**、**分电板** 以及 **USB转CAN (USB2CAN)** 功能集成于一体，作为机器人的“电气中转站”，负责电源分配与通信信号分发。

---

## 📖 核心功能与规格 (Specifications)

本模块作为连接电池、主控板（如香橙派5Plus）与四肢执行器的关键枢纽，核心参数如下：

### 1. 硬件参数表

| 参数类别 | 具体规格 | 备注 |
| :--- | :--- | :--- |
| **供电输入** | XT60端子, 48VDC | 连接电池 PACK |
| **5V 输出** | Type-C接口, 最高持续电流 8A | 为主控板、供电 |
| **48V 输出** | XT30 (2+2) 端子 × 4 | 分配至机器人四肢电机 |
| **通信接口** | USB2.0 (Type-C) | 连接主控板，实现 USB 转 CAN 功能 |
| **散热供电** | GH1.25 接口, 5V | 为系统风扇供电 |
| **尺寸** | 80mm × 60mm | 紧凑型设计 |

---

## 📂 仓库目录结构 (File Structure)

本仓库包含制造和使用该模块所需的全部工程文件：

```text
├── 00_Docs/                         # 文档目录
│   ├── Images/                      # 接口与渲染图
│   │   ├── RBE_Board_v2.0_interface_bottom.PNG  # 底部接口定义
│   │   ├── RBE_Board_v2.0_interface_top.PNG     # 顶部接口定义
│   │   └── RBE_Board_v2.0_render.JPEG           # 3D渲染效果图
│   ├── 3D_PCB5_11_2026-2-1.step    # 3D结构模型文件
│   └── 三合一电路V1.0硬件说明.pdf   # 详细硬件设计原理
│
├── 01_Gerber/                       # PCB制造文件
│   └── Gerber_RBE_Board_v2.0.zip    # Gerber文件压缩包
│
├── 02_Assembly/                     # 装配文件
│   ├── BOM_RBE_Board_v2.0.xlsx      # 物料清单
│   └── PickAndPlace_RBE_Board_v2.0.xlsx # 贴片坐标文件