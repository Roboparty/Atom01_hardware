# ATOM01_HARDWARE - RoboParty Humanoid Robot Open Source Project

**[中文](./README_cn.md)** | English

> **Project Introduction:** This repository serves as the core open-source hardware library for the **ATOM01** series of humanoid robots. We are committed to lowering the barrier to entry for bipedal robot development by providing a complete solution encompassing mechanical design, PCB schematics, and firmware.

---

## 📂 Repository Overview (Structure)

The project is managed hierarchically based on **version iterations**, containing two primary development branches: **V1.0** and **V2.0**.

### 📊 V1.0 vs V2.0 Feature Comparison

| Feature | V1.0 (Legacy) | V2.0 (Current / Recommended) |
| :--- | :--- | :--- |
| **Mechanical Design** | Original Design | **Reinforced Structure** |
| **Hardware Architecture** | Discrete Modules | **Highly Integrated Single Board** |
| **Core Improvements** | - | **Waist Limiting, Pin Calibration, Backplate Switch** |
| **Use Case** | Legacy User Maintenance | New User Development, Mass Production |

---

### 🔧 V1.0 (atom01_mechanic / atom01_pcb)
**Positioning:** Original version containing the early mechanical structure and discrete circuit board design.

-   **Core Components:**
    -   **Mechanical:** Basic bipedal structure design, including early assembly documentation and URDF files.
    -   **Hardware:** Separate Power and Communication boards (Roboto_Power, Roboto_Usb2Can).
-   **Target Audience:** Limited to legacy users still utilizing the first-generation hardware for reference.

### 🚀 V2.0 (roboto_origin_mechanic / roboto_origin_pcb)
**Positioning:** Brand new optimized version, comprehensively restructured for usability, stability, and integration.

#### ✨ Core Update Highlights
-   **🚀 Hardware System: Single Board Integration**
    -   **Optimization:** Integrated modules such as power management and communication interfaces into a **single core circuit board**.
    -   **Advantage:** Significantly simplifies internal cabling, reduces connector failure points, and enhances system stability and EMC (Electromagnetic Compatibility).
-   **⚙️ Mechanical System: Structural Reinforcement & Calibration Upgrade**
    -   **Waist Limiting:** Added a **mechanical limit switch** to ensure absolute safety for waist rotation angles.
    -   **Calibration Method:** Introduced **limit pin calibration** process, replacing the generic calibration method of the old version.
    -   **Arm Optimization:** Corrected issues present in the arm components of the previous version.
    -   **Backplate Switch:** Added a physical **main control board switch** to the robot's backplate.
-   **Target Audience:** All new users, developers, and users looking to experience the latest features.

---

## 📚 Quick Start

Please enter the corresponding directory based on your hardware version to obtain detailed documentation:

.  **V2.0 Users (Recommended):**
    -   **Mechanical Drawings:** Enter `V2.0/roboto_origin_mechanic/` to view assembly drawings and STL files.
    -   **PCB Files:** Enter `V2.0/roboto_origin_pcb/` to obtain Gerber files and schematics.
.  **V1.0 Users:**
    -   **Mechanical Drawings:** Enter `V1.0/atom01_mechanic/`.
    -   **PCB Files:** Enter `V1.0/atom01_pcb/`.

---

> **Note:** The mechanical structure and hardware interfaces of **V2.0 are not compatible with V1.0**. Please confirm the version before assembly or purchasing materials.