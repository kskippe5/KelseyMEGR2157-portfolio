# A11 – Motor Selection and Tensile Tester Design

## Team Members

<ul>
<li><strong style="color:#2563A6;">Kelsey Skipper</strong> – Engineering calculations, motor selection, and component analysis</li>
<li><strong style="color:#287746;">Gracie Steelmon</strong> – Motor mount CAD, assembly updates, and FEA</li>
<li><strong style="color:#B83D45;">Kaileigh Hill</strong> – Bill of materials, labor costs, documentation, and MEGR 2157 engineering drawings</li>
</ul>

## Project Objective

The objective of A11 was to continue the design of the bench-top tensile tester developed in A10. The system uses two lead screws to move a crosshead and is designed for a maximum tensile load of **2,000 N**. This phase focused on motor selection, supporting component calculations, CAD updates, structural analysis, cost estimates, and engineering drawings.

### Design Requirements

| Parameter | Value |
|---|---:|
| Maximum tensile load | 2,000 N |
| Load per lead screw | 1,000 N |
| Required factor of safety | 4 |
| Crosshead speed | 1–50 mm/min |
| Lead screw diameter | 3/8 in |
| Lead screw length used in A11 calculations | 24 in |
| Lead screw thread | 3/8-12 ACME |
| Calculated operating torque | 4.759 N·m |
| Design torque | 19.036 N·m |
| Required rotational speed | 0.473–23.62 RPM |

*The A10 documentation listed 3-ft lead screws, while A11 calculations use 24 in. The final purchased length should be confirmed against the CAD model.*

---

## 1. Engineering Calculations and Motor Selection

### 1.1 Motor Selection

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>Two <a href="https://www.mcmaster.com/6470K84/">McMaster-Carr DC gearmotors (6470K84)</a> were selected, one for each lead screw. Each motor has a listed rated torque of <strong>24.857 N·m</strong> and rated speed of <strong>31 RPM</strong>. The rated torque exceeds the calculated design torque of <strong>19.036 N·m</strong>. Operation throughout the required low-speed range still needs verification using the motor's torque-speed characteristics.</p>

<img src="https://github.com/user-attachments/assets/9a6996eb-44a8-4d83-a464-82720e6b1d81" alt="Motor selection calculations" style="max-width:100%; height:auto;">

<p><em>Figure 1: Motor selection and torque calculations.</em></p>

<img src="https://github.com/user-attachments/assets/bc217370-819a-4948-9e19-d67b5a2ef96b" alt="Selected motor specifications" style="max-width:100%; height:auto;">

<p><em>Figure 2: Selected DC gearmotor specifications.</em></p>

</div>

### 1.2 Motor Mount Analysis

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p><strong>6061-T6 aluminum</strong> was selected for the motor mounting brackets because of its strength, low weight, and machinability. The mounting bolt reactions and minimum bracket thickness were evaluated using allowable bearing stress.</p>

<img src="https://github.com/user-attachments/assets/e4f8e94c-af0f-4362-a341-dde0a9757f14" alt="Motor mount bearing stress calculations" style="max-width:100%; height:auto;">

<p><em>Figure 3: Motor mounting bracket calculations.</em></p>

</div>

### 1.3 Coupler Analysis

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>A proposed motor-to-lead-screw coupler was evaluated using torsional shear stress equations to estimate its minimum outside diameter and wall thickness. The proposed material was <strong>6061-T6 aluminum</strong>, and the motor-side opening must accommodate the selected motor's <strong>15.875 mm output shaft</strong>.</p>

<img src="https://github.com/user-attachments/assets/32f3199c-6238-4d86-8980-e942582fc552" alt="Coupler torsional calculations" style="max-width:100%; height:auto;">

<p><em>Figure 4: Coupler torsional stress calculations.</em></p>

<p>The coupler was analyzed but was not included in the submitted CAD assembly.</p>

</div>

### 1.4 Frame Connector Analysis

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>Vertical and transverse reaction forces were calculated for the frame connections based on the applied loads and motor reaction moments. These calculations were used to evaluate connector stresses and required thickness.</p>

<img src="https://github.com/user-attachments/assets/6c29c214-e570-498b-801e-90fa1341909e" alt="Frame connector calculations" style="max-width:100%; height:auto;">

<p><em>Figure 5: Frame connection calculations.</em></p>

<p>Separate corner brackets were not included in the submitted CAD assembly.</p>

</div>

### 1.5 Horizontal Frame Analysis

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>The horizontal frame members use <strong>heavy 40 Series aluminum T-slot extrusion</strong>. The loading conditions established for FEA were two <strong>1,000 N</strong> axial loads and two motor reaction moments of approximately <strong>25 N·m</strong>.</p>

<img src="https://github.com/user-attachments/assets/257fe632-75c8-437f-8d8d-da1577e5486e" alt="Horizontal frame loading calculations" style="max-width:100%; height:auto;">

<p><em>Figure 6: Horizontal frame loading calculations.</em></p>

</div>

### 1.6 Vertical Frame Analysis

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>The vertical frame members were evaluated under axial compression and transverse loading from the motor reaction moments, with a target factor of safety of <strong>4</strong>.</p>

<img src="https://github.com/user-attachments/assets/d7c3873f-7bf6-4ed2-9c3e-936bf32fc5ed" alt="Vertical frame calculations" style="max-width:100%; height:auto;">

<p><em>Figure 7: Vertical frame calculations.</em></p>

</div>

### 1.7 Floating Bearing Fit

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>An <strong>RC3 running fit</strong> was selected for the proposed floating bearing interface. The analysis considered shaft and hole tolerances, clearance limits, and mounting bolt clearance requirements.</p>

<img src="https://github.com/user-attachments/assets/bb661d98-5aed-4e39-83a1-99564ad583f8" alt="RC3 fit calculations" style="max-width:100%; height:auto;">

<p><em>Figure 8: Floating bearing RC3 fit calculations.</em></p>

<img src="https://github.com/user-attachments/assets/ef7e0db4-5df1-47b1-be97-cb71e951ad53" alt="Floating bearing mounting calculations" style="max-width:100%; height:auto;">

<p><em>Figure 9: Additional bearing mount and clearance calculations.</em></p>

<p>The floating bearing mount was analyzed but was not identified as a modeled component in the submitted assembly.</p>

</div>

### 1.8 Component and Material Selections

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<table>
<thead>
<tr><th>Component</th><th>Selected Material or Specification</th></tr>
</thead>
<tbody>
<tr><td>DC gearmotors</td><td>McMaster-Carr 6470K84</td></tr>
<tr><td>Lead screws</td><td>1080 carbon steel, 3/8-12 ACME</td></tr>
<tr><td>Lead screw nuts</td><td>SAE 932 bearing bronze</td></tr>
<tr><td>Motor mounting brackets</td><td>6061-T6 aluminum</td></tr>
<tr><td>Proposed couplers</td><td>6061-T6 aluminum</td></tr>
<tr><td>Proposed frame connectors</td><td>6061-T6 aluminum</td></tr>
<tr><td>Horizontal and vertical frame</td><td>Heavy 40 Series aluminum T-slot extrusion</td></tr>
<tr><td>Proposed floating bearing mounts</td><td>6061-T6 aluminum</td></tr>
<tr><td>Fasteners</td><td>Steel / selected stainless steel hardware</td></tr>
</tbody>
</table>

<p>These selections were based on strength, machinability, availability, and compatibility with the tensile tester. Final verification depends on the FEA results and the actual component specifications.</p>

</div>

---

## 2. SolidWorks CAD and Finite Element Analysis

### 2.1 Motor Mount Bracket and Assembly

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Using the motor mount calculations, the mounting bracket was modeled in SolidWorks and added to the existing A10 tensile tester assembly.</p>

<img src="https://github.com/user-attachments/assets/a1085504-8fa4-4a4e-b3ba-a5e19ddcca66" alt="Motor mounting bracket CAD" style="max-width:100%; height:auto;">

<p><em>Figure 10: Motor mounting bracket CAD model.</em></p>

</div>

### 2.2 Fastener Selection

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The bracket hole diameter was <strong>6.6 mm</strong>. The team selected <strong>M4 × 0.7 mm</strong>, <strong>70 mm</strong> long 18-8 stainless steel screws and matching nuts. The selected length was based on the combined component thickness, with additional thread length for nut engagement.</p>

<img src="https://github.com/user-attachments/assets/1571c766-708f-41bd-84e3-2383c41fd2ae" alt="Selected mounting screw" style="max-width:100%; height:auto;">

<p><em>Figure 11: Selected mounting screw.</em></p>

<img src="https://github.com/user-attachments/assets/3fbd0ece-8c9d-4f42-b50b-8665ed00ff3d" alt="Selected mounting nut" style="max-width:100%; height:auto;">

<p><em>Figure 12: Selected mounting nut.</em></p>

<img src="https://github.com/user-attachments/assets/755ec001-5631-436f-96a5-6d5318dd7a6d" alt="Mounting hardware dimensions" style="max-width:100%; height:auto;">

<p><em>Figure 13: Mounting hardware specifications.</em></p>

<p>The 6.6 mm holes are considerably larger than the nominal 4 mm screw diameter. The fit and bolt loading should be checked before manufacturing.</p>

</div>

### 2.3 FEA Setup

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>A SolidWorks Simulation study was created with the bottom of the bracket fixed. Two <strong>1,000 N downward loads</strong> were applied at the lead screw locations, along with a <strong>24.857 N·m</strong> motor reaction torque at the mounting regions.</p>

<img src="https://github.com/user-attachments/assets/1f53a527-4558-45c3-95c4-e20c1afe05c6" alt="FEA fixed geometry" style="max-width:100%; height:auto;">

<p><em>Figure 14: Fixed geometry for the FEA study.</em></p>

<img src="https://github.com/user-attachments/assets/335c16fd-3642-4dca-b334-5ea432f82544" alt="FEA applied forces" style="max-width:100%; height:auto;">

<p><em>Figure 15: Applied loads and motor torque.</em></p>

<img src="https://github.com/user-attachments/assets/46b9834c-2a4f-4a5f-bfaf-96e327b5e141" alt="FEA setup additional view" style="max-width:100%; height:auto;">

<p><em>Figure 16: Additional FEA setup view.</em></p>

</div>

### 2.4 Mesh

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The initial medium mesh did not generate correctly, and a coarser mesh also caused problems. After retrying the medium mesh, the simulation generated successfully.</p>

</div>

### 2.5 FEA Results

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The study was reviewed using von Mises stress, factor of safety, and strain plots.</p>

<img src="https://github.com/user-attachments/assets/2d898f73-c823-4d27-ada1-fb55e13b7eb8" alt="Von Mises stress results" style="max-width:100%; height:auto;">

<p><em>Figure 17: Von Mises stress results.</em></p>

<img src="https://github.com/user-attachments/assets/3d213265-15a0-4a0c-88ba-adc5180b6d2d" alt="Factor of safety results" style="max-width:100%; height:auto;">

<p><em>Figure 18: Factor of safety results.</em></p>

<img src="https://github.com/user-attachments/assets/bbbaa978-45cc-4060-aa4f-eca9d73241d7" alt="Strain results" style="max-width:100%; height:auto;">

<p><em>Figure 19: Strain results.</em></p>

</div>

### 2.6 Evaluation

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The simulation suggested that the applied motor torque had a greater effect on the bracket than the axial loads. A possible improvement would be to select a stronger material or revise the bracket geometry. The final design should be checked against the required factor of safety before manufacturing.</p>

</div>

---

## 3. Bill of Materials and Engineering Labor

### 3.1 Bill of Materials

The table combines the previously selected A10 components with the A11 motor and hardware selections. Prices marked with an asterisk are estimates.

| Component | Qty. | Unit Cost | Total | Supplier |
|---|---:|---:|---:|---|
| 3/8"-12 ACME Lead Screw | 2 | $35.32 | $70.64 | [McMaster-Carr](https://www.mcmaster.com/99030A993/) |
| Bronze Flange Nut | 2 | $111.78 | $223.56 | [McMaster-Carr](https://www.mcmaster.com/95120A592/) |
| T-Slot Framing | 1 | $245.87 | $245.87 | [Grainger](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48) |
| DC Gearmotor | 2 | $500.00* | $1,000.00 | [McMaster-Carr](https://www.mcmaster.com/6470K84/) |
| Thrust Bearing | 2 | $25.00* | $50.00 | [McMaster-Carr](https://www.mcmaster.com/thrust-bearings/) |
| Bronze Bushing | 2 | $5.00* | $10.00 | [McMaster-Carr](https://www.mcmaster.com/bushings/) |
| M4 × 0.7 mm, 70 mm Screws (pack of 10) | 1 pack | $12.88 | $12.88 | [McMaster-Carr](https://www.mcmaster.com/92010A819/) |
| M4 × 0.7 mm Hex Nuts (pack of 4,000) | 1 pack | $85.12 | $85.12 | McMaster-Carr |
| Assorted Mounting Hardware | 1 set | $40.00* | $40.00 | [McMaster-Carr](https://www.mcmaster.com/) |
| **Priced Material Subtotal** | | | **$1,738.07** | |

*This is a preliminary cost estimate, not a complete as-built BOM. Purchased motors, thrust bearings, bushings, and proposed components are not all shown in the current CAD assembly. Custom-fabricated parts and any additional frame connections have not been priced. The $40 hardware allowance should be checked to avoid double counting the listed screws and nuts.*

### 3.2 Engineering Labor Costs

Engineering labor was calculated at the required rate of **$35 per hour**, including the work completed in both A10 and A11.

| Team Member | A10 Hours | A11 Hours | Total Hours | Labor Cost |
|---|---:|---:|---:|---:|
| Kaileigh Hill | 4 | 4 | 8 | $280.00 |
| Kelsey Skipper | 3 | 5 | 8 | $280.00 |
| Gracie Steelmon | 5 | 5 | 10 | $350.00 |
| **Total** | **12** | **14** | **26** | **$910.00** |

**Labor Cost = Total Hours × $35/hr**

### 3.3 Total Engineering Cost

| Category | Cost |
|---|---:|
| Priced Materials | $1,738.07 |
| A10 Engineering Labor (12 hours) | $420.00 |
| A11 Engineering Labor (14 hours) | $490.00 |
| **Current Project Total** | **$2,648.07** |

*The current project total includes the materials priced so far and all reported engineering labor. It excludes unpriced custom components and additional fabrication costs.*

---

## 4. MEGR 2157 – Engineering Drawing Package

### 4.1 Objective

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>The objective of this portion was to prepare engineering drawings of the components modeled for the tensile tester and document the overall assembly. The drawings communicate dimensions, tolerances, materials, and assembly information.</p>

</div>

### 4.2 Drawing Standards

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>The drawings use <strong>third-angle projection</strong>, <strong>ASME Y14.5</strong> dimensioning and tolerancing conventions, and the following general inch tolerances:</p>

<table>
<thead><tr><th>Dimension Precision</th><th>General Tolerance</th></tr></thead>
<tbody>
<tr><td>X.X</td><td>±0.02 in</td></tr>
<tr><td>X.XX</td><td>±0.01 in</td></tr>
<tr><td>X.XXX</td><td>±0.005 in</td></tr>
</tbody>
</table>

<p>Drawing sheets include title blocks with the part or assembly name, scale, and drawing information.</p>

</div>

### 4.3 Crosshead Drawing (A10)

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>The previously completed crosshead drawing shows the part dimensions and lead screw mounting locations.</p>

<img src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8" alt="Crosshead engineering drawing" style="max-width:100%; height:auto;">

<p><em>Figure 20: Crosshead engineering drawing from A10.</em></p>

</div>

### 4.4 Motor Mount Bracket Drawing

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>A detailed drawing was prepared for the motor mounting bracket, including orthographic and isometric views, mounting holes, and dimensions.</p>

<img src="https://github.com/user-attachments/assets/974c1fb8-5c24-4379-bd07-07a4157b4e12" alt="Motor mounting bracket engineering drawing" style="max-width:100%; height:auto;">

<p><em>Figure 21: Motor mounting bracket engineering drawing.</em></p>

</div>

### 4.5 Final Assembly Drawing

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>The final SolidWorks assembly drawing shows the modeled tensile tester frame, crosshead, lead screws, bronze flange nuts, mounting brackets, and fasteners. The drawing includes an isometric view, a Bill of Materials, and numbered balloons identifying the components.</p>

<img src="https://github.com/user-attachments/assets/19210085-4985-4894-a918-28cd5d74febf" alt="Final tensile tester assembly drawing" style="max-width:100%; height:auto;">

<p><em>Figure 22: Final tensile tester assembly drawing with BOM and item balloons.</em></p>

<p>The drawing documents the current CAD assembly; components selected or analyzed but not modeled are not shown as installed.</p>

</div>

### 4.6 CAD and Drawing Files

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p><a href="https://github.com/user-attachments/files/35060613/Assem2.zip"><strong>Download SolidWorks CAD Assembly (Assem2.zip)</strong></a></p>

</div>

---

## 5. Lessons Learned

### Kelsey Skipper – Engineering Calculations

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>Through this assignment, I learned how motor torque affects the design of mechanical components and supporting structures. I gained a better understanding of bearing tolerances, torsional loading, and how hand calculations support FEA. I also learned the importance of verifying purchased component specifications before finalizing a design.</p>

</div>

### Gracie Steelmon – CAD and FEA

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Through this assignment, I improved my SolidWorks CAD skills by designing the motor mounting brackets and working with the tensile tester assembly. I became more comfortable modeling parts and understanding how they fit together. I also gained more experience setting up and troubleshooting FEA simulations.</p>

</div>

### Kaileigh Hill – BOM and MEGR 2157 Drawings

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>Through this assignment, I learned how to organize a Bill of Materials and calculate engineering labor costs. For the MEGR 2157 portion, I gained experience creating engineering drawings in SolidWorks, adding dimensions and tolerances, editing title blocks, and creating an assembly drawing with a BOM and numbered balloons.</p>

</div>

---

## 6. Project Time

### A10 and A11 Team Hours

| Team Member | A10 Hours | A11 Hours | Total Hours |
|---|---:|---:|---:|
| Kaileigh Hill | 4 | 4 | 8 |
| Kelsey Skipper | 3 | 5 | 8 |
| Gracie Steelmon | 5 | 5 | 10 |
| **Total** | **12** | **14** | **26** |

---

## 7. References and Resources

1. [McMaster-Carr – ACME Lead Screw](https://www.mcmaster.com/99030A993/)
2. [McMaster-Carr – Bronze Flange Nut](https://www.mcmaster.com/95120A592/)
3. [McMaster-Carr – DC Gearmotor](https://www.mcmaster.com/6470K84/)
4. [McMaster-Carr – M4 Mounting Screws](https://www.mcmaster.com/92010A819/)
5. [Grainger – T-Slot Framing](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)
6. SolidWorks and SolidWorks Simulation
7. *Machinery's Handbook*, 31st Edition
8. MEGR 2156 and MEGR 2157 course materials
