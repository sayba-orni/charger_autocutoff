# charger_autocutoff
This project is about designing and creating a battery charger from scratch with an auto cut-off
feature. The goal is to make a charger that works efficiently with modern battery-powered
devices while being safe and easy to use. The auto cut-off feature will stop charging when the
battery is full, preventing overcharging and extending the battery’s life.
In this repository I have uploaded all the files I created to design the pcb of the charger, which includes custom footprints of the components I used in this project as well as the schematic and pcb layout files. I used Altium designer for this project.


# Battery Charger with Automatic Cutoff

This project involves the design and implementation of a battery charging system with an automatic cutoff mechanism and a custom DC-DC buck converter. The circuit is designed to regulate the charging voltage and automatically disconnect the battery when a preset voltage threshold is reached, helping prevent overcharging.

The system uses a step-down transformer to convert 220V AC to 12V AC, followed by a full-wave bridge rectifier and a smoothing capacitor to obtain DC voltage. A buck converter then reduces the rectified voltage to approximately 12.6V for battery charging.

The automatic cutoff mechanism uses a MOSFET, relay, and adjustable potentiometer. As the battery voltage increases, the voltage at the MOSFET gate rises. Once the preset threshold is reached, the MOSFET activates the relay, disconnecting the charging path.

Two LEDs indicate the charging status:
- **Green LED:** Battery is charging.
- **Red LED:** Charging has been disconnected.

During experimental testing, the cutoff voltage was measured at **11.65V**, compared with the configured target of **11.67V**, demonstrating close agreement between the expected and measured switching thresholds.

## PCB Designs

The circuit schematics and PCB layouts were developed using **Altium Designer**.

### Battery Charger with Automatic Cutoff

![Battery Charger PCB](charger%20pcb.jpg)

### Custom DC-DC Buck Converter

![Custom Buck Converter PCB](custom%20buck%20converter%20pcb.jpg)
