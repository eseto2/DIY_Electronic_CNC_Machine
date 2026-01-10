# Introduction to DIY 3D Printed CNC Machine

## 🛠 Project Overview
This project documents the design and assembly of a low-cost, fully functional CNC machine built using **3D printed parts**, **aluminum profiles**, and **standard electronics**. It is capable of milling materials ranging from wood and MDF to acrylic and aluminum.

## ⚙️ Hardware & Electronics
The machine relies on accessible components. Below is a summary of the key parts required:


| Part | What it looks like | Amount needed |
| ------------- | ------------- | ------------- |
| [6000 holder](6000%20holder.stl) | ![6000 holder](Docs/Diagrams/6000%20holder.jpg) | 3 |
| [Ball screw block X axis flap](Ball%20screw%20block%20X%20axis%20flap.stl) | ![Ball screw block X axis flap](Docs/Diagrams/Ball%20screw%20block%20X%20axis%20flap.jpg) | 1
| [Ball screw block X axis](Ball%20screw%20block%20X%20axis.stl) | ![Ball screw block X axis](Docs/Diagrams/Ball%20screw%20block%20X%20axis.jpg) | 1
| [Ball screw block Y axis flap](Ball%20screw%20block%20X%20axis%20flap.stl) | ![Ball screw block Y axis flap](Docs/Diagrams/Ball%20screw%20block%20Y%20axis%20flap.jpg) | 2
| [Ball screw block Y axis](Ball%20screw%20block%20Y%20axis.stl) | ![Ball screw block Y axis](Docs/Diagrams/Ball%20screw%20block%20Y%20axis.jpg) | 2
| [Limit switch holder](Limit%20switch%20holder.stl) | ![Limit switch holder](Docs/Diagrams/Limit%20switch%20holder.jpg) | 3
| [X axis nut holder](X%20axis%20nut%20holder.stl) | ![X axis nut holder](Docs/Diagrams/X%20axis%20nut%20holder.jpg) | 1
| [Y axis nut holder left](Y%20axis%20nut%20holder%20left.stl) | ![Y axis nut holder left](Docs/Diagrams/Y%20axis%20nut%20holder%20left.jpg) | 1
| [Y axis nut holder right](Y%20axis%20nut%20holder%20right.stl) | ![Y axis nut holder right](Docs/Diagrams/Y%20axis%20nut%20holder%20right.jpg) | 1
| [Z axis bearing holder](Z%20axis%20bearing%20holder.stl) | ![Z axis bearing holder](Docs/Diagrams/Z%20axis%20bearing%20holder.jpg) | 1
| [Z axis nut holder](Z%20axis%20nut%20holder.stl) | ![Z axis nut holder](Docs/Diagrams/Z%20axis%20nut%20holder.jpg) | 1



### Mechanical
- **Frame:** 20x20mm Aluminum Profiles (various lengths).
- **Linear Motion:** 12mm rods, Lead screws (725mm, 515mm, 160mm), and linear bearings.
- **Drive System:** GT2 timing belts and pulleys (16T & 20T).

### Electronics
- **Controller:** Arduino Uno with CNC Shield.
- **Motors:** 4x Nema 17 Stepper Motors (1.7A).
- **Drivers:** A4988 or DRV8825 stepper drivers.
- **Spindle:** 500W Spindle or 775 DC Motor.
- **Power:** 12V Power Supply (6A recommended).

## 🖨️ 3D Printing Instructions
All structural brackets and mounts are 3D printed.
- **Material:** PETG is recommended for flexibility and durability, though PLA is sufficient.
- **Infill:** 20% - 50%.
- **Perimeters:** Minimum of 5 layers (Crucial for part strength).
- **Supports:** Required for specific orientations.

## 💻 Software & Firmware
1.  **Firmware:** **GRBL** installed on the Arduino Uno.
    - *Configuration:* Set steps/mm ($100=400, etc.) via console commands.
2.  **Control Software:** **CNCjs** is recommended for sending G-code. It is open-source, cross-platform (Windows/Mac/Linux/Raspberry Pi), and has a user-friendly interface.

## 📐 Milling Settings (Reference)
Recommended starting points for different materials:

| Material | Feed Rate | Depth of Cut | Notes |
| :--- | :--- | :--- | :--- |
| **Wood / MDF** | 800 mm/min | 3 mm | Adaptive clearing recommended |
| **Acrylic** | 500 mm/min | 1 mm |
| **Aluminum** | 800 mm/min | 0.2 mm | Spindle at full speed |

## ⚠️ Safety
- **Eye Protection:** Always wear safety glasses to protect against flying chips.
- **Emergency Stop:** Install a physical kill switch or keep the software stop button accessible.
- **Hearing Protection:** Recommended for long milling sessions.
## Videos

[![3D CNC Final test](Video.mp4)]
