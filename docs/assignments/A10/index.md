# A10 – Lead Screw Translating System Design

## Team Members

<ul><li><strong style="color:#287746;">Gracie Steelmon</strong> – Calculations and component selection</li><li><strong style="color:#B83D45;">Kaileigh Hill</strong> – Crosshead CAD and assembly</li><li><strong style="color:#2563A6;">Kelsey Skipper</strong> – FEA and engineering drawing</li></ul>

## Project Objective

<p>Design a bench-top tensile tester that applies up to <strong>2 kN</strong> using two lead screws to move a crosshead. The design must meet the strength, speed, and deflection requirements below.</p>

<table>
<thead><tr><th>Requirement</th><th>Value</th></tr></thead>
<tbody>
<tr><td>Maximum load</td><td>2 kN</td></tr>
<tr><td>Crosshead speed</td><td>1–50 mm/min</td></tr>
<tr><td>Lead screws</td><td>2; at least 18 in long</td></tr>
<tr><td>Minimum safety factor</td><td>4</td></tr>
<tr><td>Maximum crosshead deflection</td><td>0.1 mm</td></tr>
<tr><td>System</td><td>Mechanical, bench-top</td></tr>
</tbody>
</table>

## 1. Lead Screw Diameter

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The 2 kN load was divided between two lead screws, giving <strong>1,000 N per screw</strong>. Axial stress calculations used a safety factor of 4 to find the minimum diameter.</p>

<img src="https://github.com/user-attachments/assets/0bc8769c-7e0f-414c-87d1-cb67aca92aaa" alt="Figure 1" style="max-width:100%; height:auto;">

<p><em>Figure 1: Minimum lead screw diameter calculation.</em></p>

</div>

## 2. Lead Screw Rotational Speed

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>The required rotational speed was calculated from the crosshead speed of 1–50 mm/min and the lead screw pitch.</p>

<p><strong>Rotational Speed = Linear Speed / Screw Lead</strong></p>

<img src="https://github.com/user-attachments/assets/5793dd42-ea1c-4d6d-a522-5dc81a2d18b7" alt="Figure 2" style="max-width:100%; height:auto;">

<p><em>Figure 2: Rotational speed calculations.</em></p>

</div>

## 3. Lead Screw Torque and Selection

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Torque calculations considered the axial load, thread geometry, and friction to select suitable lead screws.</p>

<img src="https://github.com/user-attachments/assets/9f676d49-c27e-41a1-a888-4aa0584f988e" alt="Figure 3" style="max-width:100%; height:auto;">

<p><em>Figure 3: Lead screw torque and selection calculations.</em></p>

<h3>Selected Lead Screws</h3>

<table>
<thead><tr><th>Feature</th><th>Specification</th></tr></thead>
<tbody>
<tr><td>Thread</td><td>3/8"-12 Acme</td></tr>
<tr><td>Direction</td><td>Right-hand</td></tr>
<tr><td>Material</td><td>Carbon steel (grade to verify)</td></tr>
<tr><td>Length</td><td>3 ft</td></tr>
<tr><td>Quantity</td><td>2</td></tr>
</tbody>
</table>

<p><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr Lead Screw</a></p>

</div>

## 4. Bronze Nut Selection

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Internal thread bending stress was evaluated to check whether the selected bronze flange nuts could support the load.</p>

<img src="https://github.com/user-attachments/assets/b9c1b330-5509-4edb-b046-5df9507ad84a" alt="Figure 4" style="max-width:100%; height:auto;">

<p><em>Figure 4: Bronze flange nut calculations.</em></p>

<table>
<thead><tr><th>Feature</th><th>Specification</th></tr></thead>
<tbody>
<tr><td>Component</td><td>Acme bronze flange nut</td></tr>
<tr><td>Thread</td><td>3/8"-12 right-hand</td></tr>
<tr><td>Material</td><td>Bearing bronze</td></tr>
<tr><td>Quantity</td><td>2</td></tr>
</tbody>
</table>

<p><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr Bronze Flange Nut</a></p>

</div>

## 5. Crosshead Strength Analysis

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Beam bending calculations were used to evaluate crosshead strength under the 2 kN load with the required safety factor.</p>

<img src="https://github.com/user-attachments/assets/34af6662-71ff-4374-9932-6b10a0f673f6" alt="Figure 5" style="max-width:100%; height:auto;">

<p><em>Figure 5: Crosshead strength calculations.</em></p>

</div>

## 6. Crosshead Deflection Analysis

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>Beam deflection calculations were used to evaluate the crosshead against the maximum allowable deflection of <strong>0.1 mm</strong>.</p>

<img src="https://github.com/user-attachments/assets/f723f418-93d1-4be7-bb61-61c2c73579ab" alt="Figure 6" style="max-width:100%; height:auto;">

<p><em>Figure 6: Crosshead deflection calculations.</em></p>

</div>

## 7. Crosshead Multiview Sketch

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>A preliminary multiview sketch was created to show the crosshead dimensions and lead screw locations before CAD modeling.</p>

<img src="https://github.com/user-attachments/assets/f49ef004-394b-4722-bd9e-192b35f878ea" alt="Figure 7" style="max-width:100%; height:auto;">

<p><em>Figure 7: Preliminary crosshead multiview sketch.</em></p>

</div>

## 8. Material Cost Analysis

<p>The estimated cost of the selected commercial components is shown below.</p>

<table>
<thead>
<tr><th>Component</th><th>Qty.</th><th>Unit Cost</th><th>Total</th><th>Supplier</th></tr>
</thead>
<tbody>
<tr>
<td>3/8"-12 Acme Lead Screw</td><td>2</td><td>$35.32</td><td>$70.64</td>
<td><a href="https://www.mcmaster.com/99030A993/">McMaster-Carr</a></td>
</tr>
<tr>
<td>Bronze Flange Nut</td><td>2</td><td>$111.78</td><td>$223.56</td>
<td><a href="https://www.mcmaster.com/95120A592/">McMaster-Carr</a></td>
</tr>
<tr>
<td>T-Slot Framing</td><td>1</td><td>$245.87</td><td>$245.87</td>
<td><a href="https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48">Grainger</a></td>
</tr>
<tr>
<td><strong>Total</strong></td><td></td><td></td><td><strong>$540.07</strong></td><td></td>
</tr>
</tbody>
</table>

<p>The total excludes machining, custom parts, and additional hardware.</p>

## 9. SolidWorks CAD and Assembly

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<h3>9.1 Crosshead Modeling</h3>

<p>The crosshead was modeled in SolidWorks using the dimensions from the team's calculations. A rectangular profile was extruded, and two openings were added for the lead screws and flange nuts.</p>

<table>
<thead><tr><th>Feature</th><th>Dimension</th></tr></thead>
<tbody>
<tr><td>Length</td><td>12.00 in</td></tr>
<tr><td>Width</td><td>3.00 in</td></tr>
<tr><td>Height</td><td>3.684 in</td></tr>
<tr><td>Opening Diameter</td><td>0.510 in</td></tr>
<tr><td>Center Spacing</td><td>10.00 in</td></tr>
<tr><td>Material</td><td>A36 steel</td></tr>
</tbody>
</table>

<img src="https://github.com/user-attachments/assets/dde21ab3-a162-4c19-b113-25595c0aabb6" alt="Figure 8" style="max-width:100%; height:auto;">

<p><em>Figure 8: Initial crosshead model.</em></p>

<img src="https://github.com/user-attachments/assets/c9d4eb3e-d79a-4626-9064-69ef4d9a6c7d" alt="Figure 9" style="max-width:100%; height:auto;">

<p><em>Figure 9: Completed crosshead with lead screw openings.</em></p>

<hr>

<h3>9.2 CAD Components</h3>

<p>Manufacturer CAD models for the lead screws and bronze flange nuts were downloaded from McMaster-Carr. The T-slot framing model was obtained from Grainger.</p>

<img src="https://github.com/user-attachments/assets/67b3ee42-274f-4259-9dd5-ecd0a2453d9f" alt="Figure 10" style="max-width:100%; height:auto;">

<p><em>Figure 10: Bronze flange nut CAD model.</em></p>

<img src="https://github.com/user-attachments/assets/62e8d474-b98e-4cfc-9dce-502b1d3796c5" alt="Figure 11" style="max-width:100%; height:auto;">

<p><em>Figure 11: Acme lead screw CAD model.</em></p>

<hr>

<h3>9.3 Assembly</h3>

<p>The crosshead was inserted into a SolidWorks assembly. The bronze flange nuts were placed underneath the crosshead using concentric and coincident mates. The lead screws and T-slot framing were then added.</p>

<img src="https://github.com/user-attachments/assets/3d28f4ba-af76-4e79-ae5c-d5eaef791a7f" alt="Figure 12" style="max-width:100%; height:auto;">

<p><em>Figure 12: Crosshead and bronze flange nuts.</em></p>

<img src="https://github.com/user-attachments/assets/d78998ab-44d5-4194-861c-32d321561d8b" alt="Figure 13" style="max-width:100%; height:auto;">

<p><em>Figure 13: Lead screws aligned with the crosshead.</em></p>

<img src="https://github.com/user-attachments/assets/f0d4743e-ddaa-48bc-950b-b4cef81cd20d" alt="Figure 14" style="max-width:100%; height:auto;">

<p><em>Figure 14: Overall tensile tester CAD assembly.</em></p>

<hr>

<h3>9.4 CAD Files</h3>

<p><a href="https://github.com/user-attachments/files/34669260/Assem2.zip"><strong>Download SolidWorks CAD Assembly</strong></a></p>

</div>

## 10. Finite Element Analysis (FEA)

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<h3>10.1 Objective and Setup</h3>

<p>SolidWorks Simulation was used to evaluate stress, displacement, and factor of safety under a <strong>2,000 N</strong> load. The design required a safety factor of at least 4 and deflection below 0.1 mm.</p>

<p>A static study was created with a downward load and fixed supports at the two lead screw/nut mounting regions.</p>

<img src="https://github.com/user-attachments/assets/a7412365-4644-4086-9fd5-d6fc9a4bafea" alt="Figure 15" style="max-width:100%; height:auto;">

<p><em>Figure 15: SolidWorks FEA setup.</em></p>

<img src="https://github.com/user-attachments/assets/ef69c8be-1cc0-41e1-97b5-62ab791b058d" alt="Figure 16" style="max-width:100%; height:auto;">

<p><em>Figure 16: Applied load and fixed supports.</em></p>

<h3>10.2 Material and Mesh</h3>

<p>Material properties were assigned, and a solid mesh was generated. The mesh was refined to check the results.</p>

<img src="https://github.com/user-attachments/assets/2daa7e67-f124-4f4f-8052-2feded689d84" alt="Figure 17" style="max-width:100%; height:auto;">

<p><em>Figure 17: SolidWorks simulation mesh.</em></p>

<h3>10.3 Results and Evaluation</h3>

<p>Von Mises stress, displacement, and factor of safety were evaluated to determine whether the crosshead met the design requirements.</p>

<img src="https://github.com/user-attachments/assets/a5b6921c-4a2a-4504-be27-3a66ee103463" alt="Figure 18" style="max-width:100%; height:auto;">

<p><em>Figure 18: Crosshead FEA results.</em></p>

<img src="https://github.com/user-attachments/assets/ae881999-23fa-4953-ad09-853eed2b4715" alt="Figure 19" style="max-width:100%; height:auto;">

<p><em>Figure 19: Additional simulation results.</em></p>

<p>The simulation indicated that the selected crosshead design did not meet the structural requirements. Further changes to the geometry or material would need to be evaluated.</p>

</div>

## 11. Engineering Drawing

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>A multiview engineering drawing was created in SolidWorks with dimensions, tolerances, and a title block following ASME Y14.5 standards.</p>

<h3>General Tolerances</h3>

<table>
<thead><tr><th>Precision</th><th>Tolerance</th></tr></thead>
<tbody>
<tr><td>X.X</td><td>±0.02 in</td></tr>
<tr><td>X.XX</td><td>±0.01 in</td></tr>
<tr><td>X.XXX</td><td>±0.005 in</td></tr>
</tbody>
</table>

<img src="https://github.com/user-attachments/assets/75371664-f118-46c5-852b-8c5e30228bd8" alt="Figure 20" style="max-width:100%; height:auto;">

<p><em>Figure 20: Crosshead engineering drawing.</em></p>

</div>

## 12. Project Time and Resources

<table>
<thead><tr><th>Task</th><th>Time</th></tr></thead>
<tbody>
<tr><td>Calculations and component selection</td><td>5 hours</td></tr>
<tr><td>Crosshead CAD and assembly</td><td>1 hour</td></tr>
<tr><td>FEA and engineering drawing</td><td>3 hours</td></tr>
<tr><td>Documentation</td><td>3 hours</td></tr>
<tr><td><strong>Total</strong></td><td><strong>12 hours</strong></td></tr>
</tbody>
</table>

### Resources

- SolidWorks and SolidWorks Simulation
- McMaster-Carr
- Grainger
- Machinery's Handbook
- Course materials

## 13. Lessons Learned

<div style="background-color:#DDF3E4; padding:20px; border-radius:10px; margin:20px 0; color:#24313B;">

<p>From this assignment I have learned how to apply all of the equations and concepts we have learned in the semester thus far. This took me around 5 hours to complete all of the calculations.
</p>

</div>

<div style="background-color:#FCE3E3; padding:20px; border-radius:10px; margin:20px 0; color:#4A2424;">

<p>This project helped me understand how component dimensions affect an assembly. I gained experience using SolidWorks mates and manufacturer CAD files to assemble a mechanical system.</p>

</div>

<div style="background-color:#E8F1FA; padding:20px; border-radius:10px; margin:20px 0; color:#243B53;">

<p>This project provided experience with SolidWorks Simulation, applying loads and supports, interpreting FEA results, and creating an engineering drawing.</p>

</div>

## 14. References

1. Machinery's Handbook, 31st Edition.
2. Engineering Mechanics Course Materials.
3. [McMaster-Carr – Acme Lead Screw](https://www.mcmaster.com/99030A993/)
4. [McMaster-Carr – Bronze Flange Nut](https://www.mcmaster.com/95120A592/)
5. [Grainger – T-Slot Framing](https://www.grainger.com/product/80-20-T-Slot-Framing-System-Rectangle-804T48)

The total time spent on my portion of the assignment was roughly 3 hours, seeming as I had never used SolidWorks before.
