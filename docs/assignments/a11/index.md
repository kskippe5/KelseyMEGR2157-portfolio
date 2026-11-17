# A11 – Motor Selection

## Motor Selection and Calculations -- Kelsey Skipper

## Objective

My objective for this assignment was to perform the engineering calculations necessary to support the design of the mechanical tensile tester. This included motor and material selection, motor mount bearing stress analysis, coupler torsional stress analysis, frame reaction force calculations, and floating bearing fit tolerances. I also established the loading conditions for my teammates' finite element analyses and updated the bill of materials. These calculations were performed to evaluate the design's ability to withstand a maximum tensile load of 2 kN while maintaining a minimum factor of safety of 4.

## Analyze

### Design Parameters

Using the calculations completed in Part 1, I established the following design parameters:

| Parameter | Value |
|---|---:|
| Maximum tensile load | 2,000 N |
| Load per leadscrew | 1,000 N |
| Factor of safety | 4 |
| Leadscrew diameter | 3/8 in |
| Leadscrew length | 24 in |
| Thread specification | 3/8-12 ACME |
| Operational torque | 4.759 N·m |
| Required design torque | 19.036 N·m |
| Rotational speed | 0.473–23.62 RPM |

### Motor Selection

I selected two McMaster-Carr DC gearmotors (6470K84), one for each leadscrew. Each motor has a listed rated torque of 24.857 N·m and a rated speed of 31 RPM. The rated torque exceeds the calculated design torque requirement. Low-speed operation and the complete torque-speed relationship require further verification.

<img width="3094" height="4641" alt="IMG_7871" src="https://github.com/user-attachments/assets/9a6996eb-44a8-4d83-a464-82720e6b1d81" />

<img width="377" height="284" alt="Screenshot 2026-11-16 214242" src="https://github.com/user-attachments/assets/bc217370-819a-4948-9e19-d67b5a2ef96b" />

### Motor Mount

I selected Aluminum 6061-T6 for the motor mounts due to its strength, low weight, and machinability. I analyzed the reaction forces acting on the mounting bolts and calculated the minimum plate thickness based on allowable bearing stress.

<img width="3641" height="3134" alt="IMG_7872" src="https://github.com/user-attachments/assets/e4f8e94c-af0f-4362-a341-dde0a9757f14" />

### Coupler

I analyzed the coupler using torsional shear stress equations to determine the minimum outer diameter and wall thickness. Aluminum 6061-T6 was selected as the coupler material. The motor-side bore must accommodate the selected motor's 15.875 mm output shaft.

<img width="3504" height="4484" alt="IMG_7873" src="https://github.com/user-attachments/assets/32f3199c-6238-4d86-8980-e942582fc552" />

### Frame Connectors

I calculated the vertical and transverse reaction forces acting on the frame connectors due to the axial loads and motor reaction moments. These forces were used to determine the stresses acting on the connectors and evaluate their required thickness.

<img width="3340" height="4556" alt="IMG_7874" src="https://github.com/user-attachments/assets/6c29c214-e570-498b-801e-90fa1341909e" />

### Horizontal Frame Analysis

The horizontal frame consists of heavy 40 Series aluminum T-slot extrusion. The loading conditions for the finite element analysis consist of two 1,000 N axial loads and two motor reaction moments of approximately 25 N·m.

<img width="3709" height="3083" alt="IMG_7875" src="https://github.com/user-attachments/assets/257fe632-75c8-437f-8d8d-da1577e5486e" />

### Vertical Frame Analysis

The vertical frame members were analyzed under axial compression and transverse loading resulting from the motor reaction moments. The objective of the analysis was to verify that the frame maintains a minimum factor of safety of 4.

<img width="3796" height="3391" alt="IMG_7876" src="https://github.com/user-attachments/assets/d7c3873f-7bf6-4ed2-9c3e-936bf32fc5ed" />

### Floating Bearing Mount

I selected an RC3 running fit for the floating bearing interface to allow rotation without excessive clearance. I determined the shaft and hole tolerances, minimum and maximum clearances, and mounting bolt clearance requirements.

<img width="1985" height="4967" alt="IMG_7877" src="https://github.com/user-attachments/assets/bb661d98-5aed-4e39-83a1-99564ad583f8" />

<img width="2101" height="2043" alt="IMG_7878" src="https://github.com/user-attachments/assets/ef7e0db4-5df1-47b1-be97-cb71e951ad53" />

## Decide

Based on the preliminary engineering calculations, the following components and materials were selected:

| Component | Selection |
|---|---|
| Motors | McMaster-Carr 6470K84 |
| Leadscrews | 1080 carbon steel |
| Leadscrew nuts | SAE 932 bearing bronze |
| Motor mounts | Aluminum 6061-T6 |
| Couplers | Aluminum 6061-T6 |
| Frame connectors | Aluminum 6061-T6 |
| Horizontal frame | Heavy 40 Series aluminum extrusion |
| Vertical frame | Heavy 40 Series aluminum extrusion |
| Floating bearing mounts | Aluminum 6061-T6 |
| Fasteners | Steel |

These selections were made based on strength, machinability, availability, and compatibility with the existing assembly. Final verification is dependent on the FEA results, actual component dimensions, motor operating characteristics, and leadscrew capacity.

## Communicate

### Bill of Materials

| Component | Qty. | Unit Cost | Total | Supplier |
|---|---:|---:|---:|---|
| 3/8"-12 Acme Lead Screw | 2 | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| Bronze Flange Nut | 2 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| DC Gearmotor | 2 | $500.00* | $1,000.00 | [McMaster-Carr](https://www.mcmaster.com/6470K84/) |
| Thrust Bearing | 2 | $25.00* | $50.00 | [McMaster-Carr](https://www.mcmaster.com/thrust-bearings/) |
| Bronze Bushing | 2 | $5.00* | $10.00 | [McMaster-Carr](https://www.mcmaster.com/bushings/) |
| Assorted Mounting Hardware | 1 set | $40.00* | $40.00 | [McMaster-Carr](https://www.mcmaster.com/) |
| **Total** | | | **$1,394.20** | |

*Prices marked with an asterisk are estimated and subject to supplier verification.*

### Lessons Learned

Through this assignment, I learned how motor torque influences the design of mechanical components and supporting structures. I also gained a better understanding of bearing tolerances, torsional loading, and how hand calculations can be used alongside FEA to evaluate a mechanical system. Additionally, I learned the importance of verifying purchased component specifications before finalizing a design.

### Time Spent
The total time spent on my portion of this assignment was roughly 5 hours to complete all of the calculations and select the motor.
