# pcb-variable-capacitor
An Variable Capacitor Kit made of stacked PCB's


## Motivation
High voltage variable capacitors are required for tuning magnetic loop antennas. This kind of variable capacitor is often expensive and hard to find. This project aims to provide a low-cost alternative that can be easily built using PCB technology.


## Design

Based on Air Variable Capacitor, the design consists of multiple PCB's stacked together to create a variable capacitor.
The PCB's are designed with interleaving fingers that can be rotated to change the capacitance. 


## BOM
- 2 `front_rear_panel` PCB's 
- 1 or more `rotor` PCB's
- 1 or more `plate` PCB's
- 1 spacer PCB per plate PCB + 2 spacer PCB's per rotor PCB
- 5x M3 screws
- 10x M3 nuts
- solder paste and hot air gun (Optional)


## Capacitance

| Rotors | Plates | Max C, No Additional Spacers | Max C @ 1.0 mm additional spacers |
| -----: | -----: | ------------------: | -----------------: |
|      1 |      2 |           48.93 pF |           15.73 pF |
|      2 |      3 |           97.87 pF |           31.46 pF |
|      3 |      4 |          146.80 pF |           47.19 pF |
|      4 |      5 |          195.74 pF |           62.92 pF |
|      5 |      6 |          244.67 pF |           78.65 pF |


## Images
### Front and Rear Plate

![Front and Rear Plate](front_rear_plate.png)

### Plate
![Plate](plate.png)
### Rotor
![Rotor](rotor.png)
### Spacers
![Spacers](spacers.png)

