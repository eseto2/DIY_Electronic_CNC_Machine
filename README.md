# Introduction to DIY 3D Printed CNC Machine
Yes, 3D printed parts are definitely strong enough for such a CNC machine. I use 3 perimeters and 40% infill to print those parts out of PLA, PETG is also a good choice. Above you can find STL files and STEP files in case you want to modify something.
You can also buy the fully printed and assembled 3D printed CNC machine if you email me @ eovuede97@gmail.com.


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

# DIY 3D Printed CNC Machine

## 🛠 Project Overview
This project documents the design and assembly of a low-cost, fully functional CNC machine built using **3D printed parts**, **aluminum profiles**, and **standard electronics**. [cite_start]It is capable of milling materials ranging from wood and MDF to acrylic and aluminum[cite: 245, 249, 251].

## ⚙️ Hardware & Electronics
The machine relies on accessible components. [cite_start]Below is a summary of the key parts required[cite: 5, 29]:

### Mechanical
- [cite_start]**Frame:** 20x20mm Aluminum Profiles (various lengths)[cite: 8].
- [cite_start]**Linear Motion:** 12mm rods, Lead screws (725mm, 515mm, 160mm), and linear bearings[cite: 14, 17, 20].
- [cite_start]**Drive System:** GT2 timing belts and pulleys (16T & 20T)[cite: 26, 27].

### Electronics
- [cite_start]**Controller:** Arduino Uno with CNC Shield[cite: 31, 35].
- [cite_start]**Motors:** 4x Nema 17 Stepper Motors (1.7A)[cite: 30].
- [cite_start]**Drivers:** A4988 or DRV8825 stepper drivers[cite: 34].
- [cite_start]**Spindle:** 500W Spindle or 775 DC Motor[cite: 41].
- [cite_start]**Power:** 12V Power Supply (6A recommended)[cite: 213].

## 🖨️ 3D Printing Instructions
All structural brackets and mounts are 3D printed.
- [cite_start]**Material:** PETG is recommended for flexibility and durability, though PLA is sufficient[cite: 46].
- [cite_start]**Infill:** 20% - 50%[cite: 44].
- [cite_start]**Perimeters:** Minimum of 5 layers (Crucial for part strength)[cite: 45].
- [cite_start]**Supports:** Required for specific orientations[cite: 47].

## 💻 Software & Firmware
1.  [cite_start]**Firmware:** **GRBL** installed on the Arduino Uno[cite: 110].
    - [cite_start]*Configuration:* Set steps/mm ($100=400, etc.) via console commands[cite: 120].
2.  **Control Software:** **CNCjs** is recommended for sending G-code. [cite_start]It is open-source, cross-platform (Windows/Mac/Linux/Raspberry Pi), and has a user-friendly interface[cite: 220, 222, 223].

## 📐 Milling Settings (Reference)
Recommended starting points for different materials:

| Material | Feed Rate | Depth of Cut | Notes |
| :--- | :--- | :--- | :--- |
| **Wood / MDF** | 800 mm/min | 3 mm | [cite_start]Adaptive clearing recommended [cite: 246, 248] |
| **Acrylic** | 500 mm/min | [cite_start]1 mm | [cite: 250] |
| **Aluminum** | 800 mm/min | 0.2 mm | [cite_start]Spindle at full speed [cite: 251, 252] |

## ⚠️ Safety
- [cite_start]**Eye Protection:** Always wear safety glasses to protect against flying chips[cite: 231].
- [cite_start]**Emergency Stop:** Install a physical kill switch or keep the software stop button accessible[cite: 233].
- [cite_start]**Hearing Protection:** Recommended for long milling sessions[cite: 236].
## Videos

[![3D CNC Final test](Video.mp4)]
