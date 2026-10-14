# STM32 Custom Development Board

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)](https://opensource.org/licenses/MIT)
[![KiCad](https://img.shields.io/badge/KiCad-FFFFFF?style=flat-square&logo=kicad&logoColor=blue)](https://www.kicad.org/)
[![STM32](https://img.shields.io/badge/STM32-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)](https://www.st.com/)

A custom-designed printed circuit board (PCB) for an STM32 microcontroller, featuring full schematic capture, layout, and manufacturing-ready fabrication files.

##  Table of Contents
- [About the Project](#about-the-project)
- [Tech Stack](#tech-stack)
- [Getting Started](#getting-started)
- [Repository Structure](#repository-structure)


##  About the Project

This project contains the complete hardware design files for a custom STM32-based development board. It serves as a physical hardware platform for embedded C programming, control systems testing, and peripheral integration. The board was routed with a focus on signal integrity, proper grounding, and efficient power distribution.

### Tech Stack
*   **EDA Software:** KiCad (for schematic capture and PCB layout)
*   **Hardware Target:** STM32 Microcontroller

##  Getting Started

Follow these instructions to view or modify the hardware design files locally.

### Prerequisites

*   [KiCad EDA](https://www.kicad.org/download/) (Version 7.0 or higher recommended) to open the schematic and board files.
*   A Gerber viewer (if you only want to inspect the manufacturing layers).

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/MohamedHassanExp/STM-board.git
2. Navigate to the project directory
   ```bash
   cd STM-board-main
3. Open `stm board.kicad_pro` project file using KiCad.

## Repository Structure

The repository is organized to separate the editable design files from the static manufacturing outputs:

*   **Design Files:**
     The root directory contains the core KiCad project files, including the schematic (stm board.kicad_sch) and the physical layout (stm board.kicad_pcb).
*    **Board Renders:**
      High-resolution 3D renders of the physical layout are available as stm board-front.png and stm board-back.png.  
*    **Manufacturing Files (/Manufacturing/):** 
      This directory contains everything a fabrication house like JLCPCB or PCBWay needs to manufacture and assemble the board:
      * **stm board-gerber.rar:** The compressed Gerber layers and drill files for PCB fabrication.
      * **stm board-BOM.csv:** The complete Bill of Materials for component sourcing and assembly.
      * **stm board-position.csv:** The centroid/pick-and-place data for automated SMD assembly.
