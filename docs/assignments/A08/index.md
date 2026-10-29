# MEGR 2156 & 2157 — Gearbox Design and Assembly

## Objective

The objective of this project was to design, model, assemble, and analyze a functional gearbox using Autodesk Fusion. My gearbox consists of an input shaft, output shaft, two spur gears, a two-piece housing, and two journal bearings.

Throughout this project, I created individual CAD components, established assembly relationships, and checked that the gears and shafts were properly aligned. I also evaluated the design for interference and developed calculations to analyze shaft stresses, bearing pressure, surface velocity, and PV ratings.

For MEGR 2157, I expanded my work to include detailed engineering drawings of the individual components and the complete assembly. These drawings were required to follow ASME Y14.5 standards, use third-angle projection, and include appropriate tolerances for critical features.

My overall goal was to develop a gearbox design that could be assembled, manufactured, and evaluated using engineering design principles.

---

## Analyze

### 1. Gearbox Design Specifications

I began by identifying the major components and dimensions needed for my gearbox. I used two spur gears connected to separate shafts, with the smaller gear serving as the input and the larger gear serving as the output.

I used the following initial specifications:

| Parameter | Value |
|---|---|
| Input shaft diameter | 0.125 in |
| Output shaft diameter | 0.250 in |
| Input gear teeth | 18 |
| Output gear teeth | 48 |
| Diametral pitch | 48 teeth/in |
| Pressure angle | 20° |
| Input gear pitch diameter | 0.375 in |
| Output gear pitch diameter | 1.000 in |
| Gear center distance | 0.6875 in |
| Gear ratio | 2.667:1 |
| Preliminary shaft length | 1.000 in |
| Housing wall thickness | 0.250 in |
| Preliminary gear clearance | 0.100 in |

I used these values to establish the initial geometry of my gearbox and determine how the individual components would fit together.

<img width="196" height="364" alt="Screenshot 2026-10-28 182144" src="https://github.com/user-attachments/assets/4b107f2a-87ef-4591-94cc-5cd9e1607fa0" />

### 2. Gear Design and Calculations

I calculated the gear ratio, pitch diameters, and center distance using the number of teeth and diametral pitch.

I determined that my gearbox has a theoretical gear ratio of 2.667:1. This means the output shaft rotates at approximately 37.5% of the input shaft speed, while the output torque increases by a factor of approximately 2.667 under ideal conditions.

I calculated the input gear pitch diameter to be 0.375 in and the output gear pitch diameter to be 1.000 in. Using these values, I determined that the theoretical center distance between the gears should be 0.6875 in.

<img width="601" height="377" alt="Screenshot 2026-10-29 022501" src="https://github.com/user-attachments/assets/3b2bce33-5a58-4b3c-8340-a7cd32037abd" />

### 3. CAD Modeling and Assembly

I created and assembled the gearbox components using Autodesk Fusion.

I modeled the input and output shafts as separate components and positioned them concentrically with their corresponding gears. I used rigid joints to connect each shaft to its gear so that they would move together.

During the assembly process, I encountered difficulties positioning the components using rigid joints. Some components returned to their original locations after I confirmed the joint instead of remaining where I had positioned them.

To correct this, I adjusted the joint origins, alignment, and offsets until the components were positioned correctly.

<img width="1280" height="686" alt="Screenshot 2026-10-28 182829" src="https://github.com/user-attachments/assets/570d2b41-c415-48f1-8db7-7ec783df668f" />

### 4. Bottom Housing Design

I designed the bottom housing to contain the gearbox components while providing adequate space for the gears to rotate.

I began by creating a rectangular sketch and extruding it to form the base of the housing. I then created an additional rectangular profile to form the surrounding walls and interior cavity.

I selected a preliminary wall thickness of 0.250 in and positioned the interior cavity around the gear assembly to provide clearance between the gears and the housing.

I also incorporated circular openings at the shaft center locations to accommodate the input and output shafts.

<img width="1280" height="685" alt="Screenshot 2026-10-28 183507" src="https://github.com/user-attachments/assets/0d052bce-4ed8-4e6e-84ea-7d2ffccbfc59" />

<img width="1280" height="726" alt="Screenshot 2026-10-28 183837" src="https://github.com/user-attachments/assets/b9d6ff39-2e76-43d0-9731-2b221e631cba" />

<img width="1280" height="727" alt="Screenshot 2026-10-28 184435" src="https://github.com/user-attachments/assets/ea983bf2-c986-412e-8d8f-24ebbab684f8" />

### 5. Top Housing Design

I created the top housing as a separate component to enclose the gearbox and provide additional support for the shafts.

I based the geometry of the top housing on the bottom housing to maintain proper alignment between the two components.

I created circular openings at the input and output shaft locations so the shafts could extend through the housing.

I then positioned the top housing over the bottom housing to form the complete enclosure.

I chose a two-piece housing configuration because it allows the internal gearbox components to be accessed during assembly and maintenance.

<img width="1278" height="620" alt="Screenshot 2026-10-28 185517" src="https://github.com/user-attachments/assets/91640640-6231-4d5d-ad88-59da9dced8ed" />

<img width="1280" height="726" alt="Screenshot 2026-10-28 185806" src="https://github.com/user-attachments/assets/08e1f99b-d5a6-492f-9b93-0d214b0455cc" />

<img width="1280" height="620" alt="Screenshot 2026-10-28 192212" src="https://github.com/user-attachments/assets/c3e98596-65b7-4969-99ef-03a526abeb5d" />

### 6. Interference Analysis

After assembling the gearbox, I performed an interference analysis in Autodesk Fusion to identify any potential geometric conflicts between the components.

The interference inspection returned the following result:

**No interferences detected.**

Based on this result, I determined that Fusion did not identify solid-body overlap among the selected components during the inspection.

Although the inspection did not identify any interferences, I still needed to consider running clearances, shaft alignment, and bearing fits to ensure that the gearbox could operate properly.

<img width="2048" height="989" alt="nointerference detected" src="https://github.com/user-attachments/assets/32813fec-a969-41f5-b5c9-3b42a7a39742" />

### 7. Input Shaft Stress Analysis — Power Transmission

I analyzed the input shaft to determine whether my selected diameter of 0.125 in would be sufficient to withstand the forces generated during power transmission.

I considered the torsional loading caused by the input torque and the bending loads generated by the gear forces.

For my analysis, I developed equations for the tangential gear force, radial gear force, bending stress, torsional shear stress, and combined von Mises stress.

I used the factor of safety as the criterion for determining whether my shaft diameter was sufficient.

**Known Values:**

- Shaft diameter: 0.125 in
- Preliminary shaft length: 1.000 in
- Gear pitch diameter: 0.375 in
- Gear pitch radius: 0.1875 in
- Gear pressure angle: 20°

**Unknown Values:**

- Applied input torque
- Maximum bending moment
- Maximum combined stress
- Shaft material yield strength
- Factor of safety

<img width="599" height="339" alt="image" src="https://github.com/user-attachments/assets/e541f859-b01b-42f3-b3eb-c2bc8abf5544" />

**Shaft Diameter Evaluation:**

I initially selected an input shaft diameter of 0.125 in. To determine whether this diameter is sufficient, I must compare the calculated equivalent stress to the allowable stress for my selected material.

If the calculated factor of safety does not meet the required design value, I will need to increase the shaft diameter.

### 8. Output Shaft Stress Analysis — Short Shaft

I analyzed the output shaft using the same general approach as the input shaft.

For my design, I selected an output shaft diameter of 0.250 in. Because the gearbox reduces rotational speed, the output shaft experiences increased torque compared to the input shaft.

I considered the output torque, gear forces, bending stress, torsional shear stress, and combined von Mises stress.

**Known Values:**

- Shaft diameter: 0.250 in
- Preliminary shaft length: 1.000 in
- Gear pitch diameter: 1.000 in
- Gear pitch radius: 0.500 in
- Gear ratio: 2.667:1

**Unknown Values:**

- Applied output torque
- Maximum bending moment
- Maximum combined stress
- Shaft material yield strength
- Factor of safety

<img width="601" height="329" alt="image" src="https://github.com/user-attachments/assets/4595898e-44f4-4031-bd91-2b48a3948cb7" />

**Shaft Diameter Evaluation:**

I selected a larger diameter for the output shaft because it must transmit more torque than the input shaft.

Since torsional stress decreases as shaft diameter increases, the 0.250-in shaft provides greater resistance to torsional loading.

I will use my calculated equivalent stress and factor of safety to determine whether the selected diameter is sufficient or whether I need to modify it.

### 9. Journal Bearing Design — Pressure, Velocity, and PV Rating

I evaluated journal bearings as a method of supporting the rotating shafts inside the gearbox housing.

The purpose of these bearings is to provide radial support while allowing the shafts to rotate.

To evaluate the bearings, I considered the projected bearing pressure, surface velocity, and PV rating.

I used the PV rating to determine whether the selected bearing material would be suitable for the expected operating conditions.

**Known Values:**

- Input shaft diameter: 0.125 in
- Output shaft diameter: 0.250 in
- Gear ratio: 2.667:1
- Preliminary bearing length-to-diameter ratio: 1:1

**Unknown Values:**

- Actual radial bearing loads
- Operating rotational speeds
- Final bearing lengths
- Bearing pressure
- Surface velocity
- PV rating
- Allowable bearing material ratings

<img width="592" height="513" alt="image" src="https://github.com/user-attachments/assets/3b04ea23-696e-4347-be07-01a1ddc95d33" />

**Bearing Material Selection:**

I considered oil-impregnated bronze as a potential bearing material because it is commonly used in sleeve bearing applications and provides favorable friction and wear characteristics.

To finalize my material selection, I will compare my calculated pressure, velocity, and PV values to the allowable ratings provided in the course material.

### 10. Journal Bearing Wall Thickness

I evaluated the wall thickness of the journal bearings to determine whether the sleeves would provide adequate structural support.

I defined the bearing wall thickness using the difference between the outer diameter and inner diameter of each sleeve.

My goal was to select a thickness that would provide sufficient material around the shaft while maintaining compatibility with the housing.

**Known Values:**

- Input bearing nominal inner diameter: 0.125 in
- Output bearing nominal inner diameter: 0.250 in
- Candidate bearing material: oil-impregnated bronze

**Unknown Values:**

- Final bearing outer diameters
- Required bearing wall thicknesses
- Applied bearing loads
- Allowable material stress

### 11. Journal Bearing Component Selection

I considered commercially available journal bearings from McMaster-Carr to reduce the amount of custom manufacturing required for my gearbox.

I needed two sleeve bearings: one for the input shaft and one for the output shaft.

When selecting the bearings, I considered their inner diameters, outer diameters, lengths, materials, and operating ratings.

**Input Journal Bearing**

<img width="346" height="182" alt="image" src="https://github.com/user-attachments/assets/7dc266a8-d45f-4b89-a1f1-598cbe947daf" />

Component Name: Oil-Embedded 841 Bronze Sleeve Bearing for 3/8" Shaft Diameter and 1/2" Housing ID, 7/8" Long

Part Number: 6391K111

Inner Diameter: 0.125 in

Outer Diameter: 0.250 in

Length: 0.250 in

**Output Journal Bearing**

<img width="347" height="206" alt="image" src="https://github.com/user-attachments/assets/ae0a96a3-99ea-4ad1-a1f3-2f7368f3d335" />

Component Name: Oil-Embedded 841 Bronze Flanged Sleeve Bearing for Food and Beverage, for 1/4" Shaft Diameter, 3/8" Long

Part Number: 3746K3

Inner Diameter: 0.250 in

Outer Diameter: 0.375 in

Length: 0.375 in

### 12. Engineering Drawings and Dimensioning

For the MEGR 2157 portion of this project, I was required to create engineering drawings for the individual gearbox components and the complete assembly.

My drawing deliverables consisted of six multiview part drawings and one assembly drawing.

I used third-angle projection and followed ASME Y14.5 standards for dimensioning and tolerancing.

The required drawings were:

1. Input shaft
2. Output shaft
3. Bottom housing
4. Top housing
5. Input journal bearing
6. Output journal bearing
7. Complete gearbox assembly

I included the dimensions necessary to define each component's geometry and communicate the information needed for manufacturing.

### 13. Dimensioning and Tolerancing

I used third-angle projection for my engineering drawings and applied the general tolerance block specified in the assignment.

**General Tolerance Block:**

| Decimal Places | Tolerance |
|---|---|
| X.X | ±0.02 in |
| X.XX | ±0.01 in |
| X.XXX | ±0.005 in |

I used these general tolerances unless a different tolerance was specified for a particular feature.

I also identified critical features that required more specific tolerances.

For my gearbox, I considered the shaft-to-bearing interfaces and the shaft center locations to be particularly important.

I needed to ensure that the shafts could rotate within their bearings without excessive clearance or interference.

I also needed to maintain the proper center distance between the shafts so that the gears would mesh correctly.

---

## Decide

### Gear and Shaft Selection

I selected an 18-tooth input gear and a 48-tooth output gear to produce a theoretical gear ratio of 2.667:1.

I modeled the input shaft with a diameter of 0.125 in and the output shaft with a diameter of 0.250 in.

I chose the larger output shaft diameter because the output shaft must transmit increased torque.

To verify my selections, I developed stress equations for both shafts and evaluated their expected loading conditions.

### Housing Configuration

I decided to use a rectangular, two-piece housing because it provided a straightforward way to enclose the gears and support the shafts.

I separated the housing into top and bottom components so the internal components could be accessed during assembly and maintenance.

I selected a preliminary wall thickness of 0.250 in and designed the interior cavity around the gear assembly.

### Journal Bearing Selection

I chose sleeve-style journal bearings as my preliminary bearing configuration.

I considered oil-impregnated bronze because it is commonly used for rotating shaft applications.

I used the pressure, velocity, PV, and wall thickness calculations to establish the requirements for my final bearing selection.

### Engineering Drawing Decisions

I used third-angle projection to satisfy the assignment requirements.

I applied the specified general tolerance block and identified critical shaft and bearing features that required individual tolerances.

I focused on these features because their dimensional accuracy directly affects the fit, alignment, and operation of the gearbox.

### Design Verification

I used Autodesk Fusion's interference inspection to evaluate my assembled gearbox.

The inspection reported no interferences among the selected components.

Based on this result, I retained my preliminary assembly configuration while continuing to evaluate the shaft stresses, bearing requirements, and critical dimensions.

---

## Communicate

### Final Design Summary

Throughout this project, I developed a gearbox assembly in Autodesk Fusion consisting of two spur gears, an input shaft, an output shaft, and a two-piece housing.

I selected an 18-tooth input gear and a 48-tooth output gear, resulting in a theoretical gear ratio of 2.667:1.

I modeled the shafts and used rigid joints to connect them to their corresponding gears. I also designed the top and bottom housing components to enclose the gearbox while allowing the shafts to extend through the housing.

After completing the assembly, I performed an interference analysis and received a result of no interferences detected.

I developed the mechanical analysis for the input and output shafts and evaluated the requirements for journal bearing pressure, velocity, PV rating, and wall thickness.

For MEGR 2157, I also prepared the engineering drawing requirements for the individual components and complete assembly, including third-angle projection, dimensional tolerances, and critical-feature callouts.

### Design Challenges and Revisions

One of the main challenges I encountered was positioning the components correctly within the Autodesk Fusion assembly.

When I initially created rigid joints, some components returned to their previous locations rather than remaining where I wanted them.

I corrected these issues by adjusting the joint origins, offsets, and component alignment.

I also had to make adjustments while designing the housing to ensure that the shaft openings aligned with the shafts and that the interior provided enough clearance for the gears.

These challenges helped me better understand how component relationships and geometric constraints affect the overall assembly.

Lessons Learned

Through this project, I improved my understanding of gearbox design, CAD assemblies, and mechanical analysis. I gained experience creating rigid joints, positioning gears and shafts, designing housings, and checking for interference in Autodesk Fusion.

I also learned how shaft stress calculations and journal bearing requirements influence component dimensions and material selection. The engineering drawing portion reinforced the importance of proper dimensioning and tolerancing when communicating a design for manufacturing.

Overall, this project helped me connect mechanical design calculations with CAD modeling and engineering documentation.

Final Deliverables

<img width="1280" height="620" alt="Screenshot 2026-10-28 192212" src="https://github.com/user-attachments/assets/56039b24-2202-4037-9672-5a2a1bb9201b" />

Final Engineering Drawings:
<https://a360.co/4e3TZyj>
<https://a360.co/4yS6zYJ>
<https://a360.co/3WdLPx7>
<https://a360.co/3WTRuIT>
<https://a360.co/4zfYi1Z>
<https://a360.co/4f0ZiPg>
<https://a360.co/4iu5IHT>

Final CAD Model:
<https://a360.co/4yNjcUW>

Time Spent:
In total, this assignment took me about five hours to do. I thought I had to revolve the shafts. I did not!



