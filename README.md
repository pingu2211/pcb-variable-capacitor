# pcb-variable-capacitor
An Variable Capacitor Kit made of stacked PCB's


## Motivation

High voltage variable capacitors are required for tuning magnetic loop antennas. This kind of variable capacitor is often expensive and hard to find. This project aims to provide a low-cost alternative that can be easily built using PCB technology.

### Cost
#### PCB's 

In early april 2026, I ordered the PCB's for this project from JLCPCB, a popular PCB manufacturer. The total cost for the PCB's was around USD$70 for 10 capacitors (excluding shipping). 

## Design

Based on Air Variable Capacitor, the design consists of multiple PCB's stacked together to create a variable capacitor.
The PCB's are designed with interleaving fingers that can be rotated to change the capacitance. 


## General BOM
### PCB's

- 2 `front_rear_panel` PCB's 
- 1 or more `rotor` PCB's (see theoretical capacitance table below)
- 1 or more `plate` PCB's (see theoretical capacitance table below)
- 1 `spacer` PCB per plate PCB
- 2 `spacer` PCB's per rotor PCB

### Other Components

- 2 M3 spring washers
- 4 M3 x 40mm screws (for 5 rotor and 6 plate, 1mm spaced configuration, adjust accordingly for different configurations)
- 1 M3 threaded rod 
- 10 M3 nuts
- 2 M3 flat, or lock washers per spacer PCB

### Assembly Tools

- spanner or socket to fit your M3 screws and nuts
- solder paste and hot air gun (Optional)

## Construction
### Plates Assembly

Use the theoretical capacitance table to determine the number of rotor and plate PCB's needed for your desired capacitance range. For example, if you want a maximum capacitance of around 50 pF, you can use 2 rotor PCB's and 3 plate PCB's.

1. Place the 4 M3 screws through the holes in the front plate PCB's.
2. Add an M3 nut to each screw, holding the front plate PCB's in place. 
3. Add a plate PCB on to the back of the front plate PCB's, ensuring that the two holes in the plate PCB's align with the screws marked `plate`.
4. Add a spacer PCB to each of the screws marked `plate`.

>! Repeat steps 3 and 4 for each additional plate PCB, ensuring that the holes align with the screws marked `plate` and that the spacer PCB's are placed between the plate PCB's as needed to achieve the desired capacitance range.

>! To achieve a 1mm spacing between the plates, place 2 M3 Spring washers between each `plate` and `spacer` PCB.

>! To achieve the lower spacing, solder the `plate` and `spacer` PCB's together rather than using spring washers. This will create a more compact assembly and allow for a higher capacitance range, although at a lower breakdown voltage.

6. Add an M3 nut to the end of the 2 screws marked `plate` and tighten to secure the assembly.

### Rotors Assembly
1. Place an M3 nut on to the end of the M3 threaded rod, at least 10mm from the end.
2. Place the M3 threaded rod through the center hole marked `rotor` in the front plate PCB.
3. Add an M3 nut to the end of the threaded rod to capture the front plate PCB.
4. Place a `spacer` PCB on the threaded rod, on the long side protruding from the nut. This should line up with the first plate PCB.
5. Add a `rotor` PCB to the threaded rod, ensuring that the holes in the rotor PCB align with the screws marked `rotor`.
6. Add another `spacer` PCB to the threaded rod
7. Repeat steps 5 and 6 for each additional rotor PCB, ensuring that the holes align with the screws marked `rotor` and that the spacer PCB's are placed between the rotor PCB's. 

>! To achieve a 1mm spacing between the plates, place 2 M3 Spring washers between each `plate` and `spacer` PCB.

>! To achieve the lower spacing, solder the `rotor` and `spacer` PCB's together rather than using spring washers. This will create a more compact assembly and allow for a higher capacitance range, although at a lower breakdown voltage.

8. Add an M3 nut to the end of the threaded rod loosely capturing the assembly.
9. Align all of the rotor PCB's, and tighten the M3 nut to secure the assembly.

>! Use a ruler, or the edge of the bench against the flat edge of the rotor PCB's and the tops of the `plate` PCB's to ensure that they are all aligned and parallel to each other.

### Final Assembly
1. Loosely add an additional M3 nut to the end of the threaded rod, and the 4 screws.
2. Add a spring washer to each of the screws and the threaded rod.
3. Place the rear plate PCB on to the back of the assembly, ensuring that the holes align with the screws and threaded rod. The holes in the rear plate PCB should align with the screws marked `plate` and the threaded rod should align with the hole marked `rotor`. Incorrect alignment of the rear plate PCB can cause the plate and rotor to short out.
4. Add a spring washer to the end of the threaded rod and each of the screws
5. Add an M3 nut to each of the screws and the threaded rod.
6. Tighten the 4 nuts on the screws to secure the rear plate PCB.
7. Adjust the nut on the threaded rod to achieve the desired tension on the rotor assembly, ensuring that the rotor PCB's are able to rotate smoothly without excessive play.

## Theoretical Capacitance

The following table shows the theoretical capacitance values for different configurations of rotors and plates, both without additional spacers and with 1.0 mm additional spacers.

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

