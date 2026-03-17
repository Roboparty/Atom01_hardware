# ROBOTO

**[中文](./README_cn.md)** | [English](./README.md)

> **项目简介：** 本项目是一个开源的双足机器人。本项目致力于降低组装门槛，提供了从机械结构到电路连接的“保姆级”装配教程。

---

## 📚 核心文档导航 (Documentation)

我们为初学者准备了详细的 PDF 手册，请**务必按照以下顺序阅读**：

| 顺序 | 文档名称 | 内容说明 | 存放位置 |
| :---: | :--- | :--- | :--- |
| 1️⃣ | **[安装手册-0317.pdf](00_Docs/安装手册-0317.pdf)** | 核心组装教程 | `00_Docs/` |
| 2️⃣ | **[Roboto_origin走线说明.pdf](00_Docs/Roboto_origin走线说明.pdf)** | 电子接线指导 | `00_Docs/` |
| 3️⃣ | **[插销标定说明.pdf](00_Docs/插销标定说明.pdf)** | 插销标定方法 | `00_Docs/` |
| 4️⃣ | **[3D打印件标定说明.pptx](00_Docs/3D打印件标定说明.pptx)** | 3D打印件标定说明 | `00_Docs/` |

---

## 📂 项目文件架构 (File Structure)

本仓库采用模块化结构，文件组织如下：

```text
├── 00_Docs/                         # [文档] 核心说明书
│   ├── 安装手册-0317.pdf            # 核心安装手册
│   ├── 插销标定说明.pdf             # 插销标定说明
│   ├── Roboto头原型机 (RoboParty Roboto Origin) 散件清单 V1.1.3.xlsx # 散件清单
│   ├── Original-0310.pdf            # 产品介绍书
│   ├── robo_origin SOP.pdf          # 标准作业程序
│   └──Roboto_origin走线说明.pdf      # 走线说明  
│
├── 01_SW_Project/                   # [源文件] solidworks工程文件
│   └── robo_origin_2.0              # Roboto Origin 2.0 工程文件
│
├── 02_Manufacturing/                # [制造] 生产加工文件
│   ├── 3D_Printing                  # 3D打印相关文件
│   └── CNC_Machining                # CNC加工相关文件
│
└── 03_URDF/                         # [仿真] 机器人描述文件
    ├── meshes                       # 仿真模型网格文件
    ├── urdf                         # URDF配置文件

