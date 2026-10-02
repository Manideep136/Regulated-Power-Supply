# Regulated-Power-Supply

Project Overview

This project is a Regulated Power Supply PCB designed using KiCad. The purpose of the circuit is to convert an unregulated DC input voltage into a stable and regulated DC output voltage.

The PCB is designed as a beginner-friendly electronics project to understand the complete PCB design process, including schematic design, component selection, footprint assignment, PCB layout, routing, ERC/DRC checking, and 3D visualization.

🎯 Objectives
Design a regulated DC power supply circuit.
Convert an input DC voltage into a stable output voltage.
Learn schematic design using KiCad.
Select appropriate footprints for electronic components.
Design and route a PCB.
Perform ERC and DRC checks.
Generate a 3D view of the completed PCB.
Understand the complete PCB design workflow.
⚡ Working Principle

The regulated power supply works in the following stages:

DC Input
An external DC voltage is supplied to the circuit through the input connector.
Filtering
Capacitors are used to reduce unwanted fluctuations and noise in the input voltage.
Voltage Regulation
A voltage regulator is used to maintain a constant output voltage even when the input voltage or load changes within the regulator's operating range.
Output Filtering
An additional capacitor helps stabilize the regulated output and reduce noise.
DC Output
The regulated voltage is available at the output connector and can be supplied to another electronic circuit.
Block Diagram
DC INPUT
   │
   ▼
Input Capacitor
   │
   ▼
Voltage Regulator
   │
   ▼
Output Capacitor
   │
   ▼
REGULATED DC OUTPUT
🧰 Components Used
Component	Quantity	Purpose
Voltage Regulator	1	Regulates the output voltage
Input Capacitor	1	Filters input voltage
Output Capacitor	1	Stabilizes output voltage
Resistors	As required	Current limiting / indication
LED	1	Power indication
Input Connector	1	DC input connection
Output Connector	1	Regulated output connection
PCB	1	Mounting and electrical connections

Note: The exact component values depend on the schematic used for this project.

🔌 Input and Output
Input

The input connector is used to provide DC power to the PCB.

INPUT
 +V  ─────────► Regulator
 GND ─────────► GND
Output

The regulator provides a stable DC voltage at the output connector.

OUTPUT
 +V_REG ──────► Load
 GND    ──────► Load

Always verify the input voltage and regulator rating before powering the PCB.

🖥️ Software Used
KiCad
KiCad Schematic Editor
KiCad PCB Editor
KiCad 3D Viewer
🧩 KiCad Design Process

The PCB was designed using the following workflow:

1. Schematic Design

The complete circuit was first created in KiCad Schematic Editor.

Components were placed and connected according to the circuit design.

2. Assign Footprints

Suitable footprints were assigned to each component according to the physical components that will be used.

Examples include:

Resistor_THT
Capacitor_THT
Package_TO_SOT_THT
Connector
LED

The exact footprint should always match the physical component purchased.

3. PCB Layout

The schematic was transferred to the PCB Editor.

Components were arranged on the PCB to obtain a compact and practical layout.

4. Routing

Tracks were created between the components according to the schematic connections.

Power and ground paths should be given appropriate track widths according to the expected current.

5. Design Rule Check

The PCB was checked using DRC (Design Rules Checker) to identify:

Unconnected tracks
Track clearance problems
Short circuits
Incorrect board geometry
Other PCB design-rule violations
6. 3D Visualization

KiCad's 3D Viewer was used to inspect the final PCB and verify component placement.

📁 Project Structure

A typical KiCad project contains:

Regulated-Power-Supply/
│
├── Regulated-Power-Supply.kicad_pro
├── Regulated-Power-Supply.kicad_sch
├── Regulated-Power-Supply.kicad_pcb
├── README.md
│
└── images/
    ├── schematic.png
    ├── pcb.png
    └── 3d-view.png
🔍 Important PCB Design Considerations
Check the polarity of capacitors.
Check the polarity of LEDs.
Verify regulator pin configuration.
Use the correct footprint for every component.
Keep power traces sufficiently wide.
Maintain proper clearance between PCB tracks.
Check all connector pin assignments.
Run ERC before PCB layout.
Run DRC after routing.
Verify the PCB using the 3D Viewer before fabrication.
🧪 Testing

After assembling the PCB:

Check the PCB visually for solder bridges and incorrect components.
Verify the polarity of all polarized components.
Check continuity between power and ground.
Apply the input voltage carefully.
Measure the output voltage using a multimeter.
Verify that the output remains close to the designed regulated voltage.
Connect the intended load and test the circuit again.
📚 What I Learned

Through this project, I learned:

How to create a schematic in KiCad.
How to select electronic components.
How to assign footprints.
How to transfer a schematic to PCB layout.
How to place components on a PCB.
How to route PCB tracks.
How to use ERC and DRC.
How to view a PCB in 3D.
How a voltage regulator is used in a power supply circuit.
Basics of designing a PCB suitable for fabrication.
🚀 Future Improvements

The project can be improved by adding:

Adjustable output voltage
Multiple output voltage levels
Reverse-polarity protection
Over-current protection
Fuse protection
Power-on LED indicator
Screw-terminal input/output
Larger heat sink for the regulator
USB output
Voltage and current display
⚠️ Safety
Do not exceed the maximum input voltage of the regulator.
Check capacitor voltage ratings before assembly.
Observe correct polarity.
Do not short-circuit the output.
If using a high-voltage AC source, use an appropriate isolated AC-to-DC stage and proper electrical safety practices. This PCB should not be connected directly to mains AC.
📸 Project Images


📌 Conclusion

The Regulated Power Supply PCB is a useful beginner KiCad project for understanding the complete PCB design process. It combines basic power-supply concepts with practical PCB design techniques such as schematic creation, footprint selection, component placement, routing, ERC, DRC, and 3D visualization.

This project provides a foundation for designing more advanced power supply, sensor, Arduino, ESP32, and IoT PCBs.

👨‍💻 Author

Manideep Kolluri

Project: Regulated Power Supply PCB
Tool: KiCad
Domain: Electronics / PCB Design
