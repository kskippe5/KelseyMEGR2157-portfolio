# MEGR 2156/2157 — Bracket Finite Element Analysis (FEA)

## Objective

The objective of this assignment is to use Finite Element Analysis (FEA) to evaluate and optimize the bracket and linkage developed in previous assignments. The goal is to improve the strength, stiffness, and weight of both components while maintaining the original material selection. Using Autodesk Fusion 360, static stress simulations will be performed to evaluate maximum von Mises stress, displacement, safety factor, and mass. Mesh convergence studies will be conducted to validate the results before making geometric modifications. Three design iterations will be evaluated for each component, with a required safety factor of 4.

## Analyze

Initial Bracket Design

The original bracket was designed to attach to a rigid T-beam while supporting a polyester strap through a lower cylindrical feature. The bracket was modeled in Autodesk Fusion 360 using Aluminum 6061, consistent with the material selected in previous assignments.

For the initial analysis, a static load of 650 lbf (2,891 N) was selected within the assignment's required range of 500–800 lbf. The load was applied downward to the cylindrical feature to represent the force transferred by the polyester strap. Fixed constraints were used to approximate the support provided by the rigid T-beam at the upper T-shaped channel.

This simplified analysis assumes the support is rigid and does not fully account for contact and sliding between the bracket and T-beam.

<img width="1280" height="764" alt="Screenshot 2026-10-21 234714" src="https://github.com/user-attachments/assets/4639252c-d265-4dd5-ad2e-c5d0b0db7793" />

<img width="695" height="472" alt="Screenshot 2026-10-22 055545" src="https://github.com/user-attachments/assets/c791ff56-769c-4332-9b5c-c11d809d8c80" />

Initial FEA Simulation — Mesh 1

The first static stress simulation was performed using the original bracket geometry. The analysis produced a maximum von Mises stress of 341.023 MPa and a minimum safety factor of 0.806.

The highest stress concentrations appeared around the vertical support connecting the upper bracket to the lower cylindrical feature. This indicated that the existing support geometry could be a critical area for improvement.

Because the minimum safety factor was below the required value of 4, the initial design did not satisfy the strength requirement under the modeled loading conditions.

<img width="1280" height="764" alt="Screenshot 2026-10-22 060655" src="https://github.com/user-attachments/assets/21cf6d92-262d-43aa-8f21-e97afd37a9f0" />

<img width="1280" height="698" alt="Screenshot 2026-10-22 060718" src="https://github.com/user-attachments/assets/6777d050-22a6-4d0f-a941-5f518bf458e5" />

Mesh 2
To evaluate the accuracy of the initial simulation, a second analysis was performed using a refined mesh. A local mesh size of approximately 3.678 mm was used to improve the resolution of the stress distribution.

The second simulation produced a maximum von Mises stress of 451.690 MPa and a maximum displacement of 2.915 mm.

The displacement results showed that the greatest deformation occurred near the free end of the lower cylindrical feature. The stress results continued to indicate significant loading in the vertical support and its connection to the upper bracket.

<img width="1278" height="702" alt="Screenshot 2026-10-22 061121" src="https://github.com/user-attachments/assets/82683c70-4e28-44f8-8aff-01e7233f802c" />

<img width="1280" height="719" alt="Screenshot 2026-10-22 061137" src="https://github.com/user-attachments/assets/f6d62ccc-10fb-46e8-9753-b48fd334dd6a" />

Mesh Convergence Analysis

Mesh convergence was evaluated by comparing the maximum von Mises stress from the first and second simulations.

<img width="190" height="159" alt="Screenshot 2026-10-22 060825" src="https://github.com/user-attachments/assets/9bc61052-8783-45b2-9286-5427a02de371" />

**Mesh 1 maximum stress:**

341.023 MPa

**Mesh 2 maximum stress:**

451.690 MPa

The difference between the two stress results was 24.50%, exceeding the required convergence tolerance of 7%. Therefore, a third simulation using a finer mesh is necessary.

If convergence is not achieved after the third attempt, the finest mesh results will be used in accordance with the assignment instructions, and the remaining uncertainty will be documented.

Mesh 3
A third static stress simulation was performed using a finer mesh to further evaluate convergence. The simulation produced a maximum von Mises stress of 719.084 MPa and a maximum displacement of 2.971 mm.

The maximum stress continued to increase with mesh refinement, while the maximum displacement changed only slightly. The displacement was greatest near the free end of the cylindrical pin, indicating bending of the lower bracket support.

The displacement results satisfied the required 7% convergence tolerance; however, the maximum stress results did not. The increasing maximum stress may be associated with a localized stress concentration or numerical singularity near the connection between the vertical support and upper bracket.

In accordance with the assignment instructions, the finest mesh results were retained after three attempts. Because stress convergence was not achieved, the reported maximum stress will be treated as a preliminary numerical result rather than a fully validated design stress.

<img width="1280" height="715" alt="Screenshot 2026-10-22 061905" src="https://github.com/user-attachments/assets/2c5d6977-51a9-4817-8e3a-2708098d0c15" />

<img width="1280" height="717" alt="Screenshot 2026-10-22 061918" src="https://github.com/user-attachments/assets/bbfa88d6-0bad-43f8-9d5e-5ff3f4d5a2e3" />

Design I Evaluation

The original bracket geometry demonstrated insufficient strength under the assumed 650 lbf loading condition. The simulations identified the vertical support and its upper connection as critical regions requiring further investigation.

The results suggest that increasing the cross-sectional area of the vertical support and introducing smoother geometric transitions could improve the structural performance.

The next design iteration will focus on reducing stress concentrations and increasing stiffness while minimizing unnecessary additional mass.

<img width="1280" height="717" alt="Screenshot 2026-10-22 061918" src="https://github.com/user-attachments/assets/d860a642-a973-42fa-baf3-fe17bdf05fa8" />

## Decide

Initial Design Evaluation

Based on the preliminary FEA results, the original bracket requires geometric improvements to satisfy the required safety factor while maintaining adequate stiffness.

The greatest concern is the elevated stress around the vertical support and its connection to the upper portion of the bracket. The initial results suggest that this region may benefit from additional material, increased thickness, or a smoother transition between features.

Before modifying the geometry, the third mesh analysis will be completed to evaluate convergence. The location of the maximum stress will also be inspected to determine whether the reported peak represents a physical stress concentration or a numerical effect caused by the mesh or boundary conditions.

Proposed Design II Modifications

For the second design iteration, I plan to strengthen the vertical support connecting the upper bracket to the cylindrical pin. Possible modifications include increasing the support thickness and adding fillets to reduce abrupt geometric transitions.

The modified design will be analyzed under the same material properties, applied load, and boundary conditions as Design I to allow a consistent comparison.

<img width="968" height="496" alt="Screenshot 2026-10-22 062118" src="https://github.com/user-attachments/assets/0d3ef56f-33e3-44c3-9004-f097fe1d9768" />

Design II — Preliminary Safety Factor Analysis

After adding a fillet underneath the main bracket body, I performed a static stress analysis using the same material and applied loading conditions as Design I.

The simulation produced a maximum von Mises stress of 624.184 MPa, a maximum displacement of 1.816 mm, and a minimum safety factor of 0.441.

Compared with the finest-mesh results from Design I, the maximum displacement decreased by approximately 38.88%, while the maximum stress decreased by approximately 13.20%.

The greatest displacement occurred near the free end of the cylindrical pin, while the highest stresses remained concentrated around the connection between the cylindrical pin and vertical support.

These preliminary results suggest that adding the fillet improved the stiffness of the bracket and may have reduced localized stress. However, the minimum safety factor remained below the required value of 4, and further mesh refinement is necessary to validate the results.

<img width="1280" height="674" alt="Screenshot 2026-10-27 205950" src="https://github.com/user-attachments/assets/800b44f9-0ad1-4b27-b6ba-4c135dfff690" />

<img width="1271" height="689" alt="Screenshot 2026-10-27 210007" src="https://github.com/user-attachments/assets/d56aebcf-b7d0-4d28-8410-4e5d8b22d357" />

After reviewing Design II results, I refined the mesh and ran it again.

<img width="584" height="388" alt="image" src="https://github.com/user-attachments/assets/c55a5d95-296d-47be-b77c-ec1ef38412c8" />

It seems promising since it stayed on this window for about 15 minutes. :D

<img width="691" height="401" alt="image" src="https://github.com/user-attachments/assets/3b77e0c2-26dd-4d59-b4e5-3ee25a25dcf5" />

dawgggg 

<img width="337" height="74" alt="image" src="https://github.com/user-attachments/assets/d99ada08-7523-43b3-8af4-25c007adbd71" />

Design III Modifications

For the third design iteration, I modified the bracket by increasing the thickness of the vertical support connecting the upper T-shaped mounting section to the lower cylindrical pin. An additional 0.20 inches of material was introduced using the Extrude feature in Autodesk Fusion 360.

This modification was selected because the previous FEA simulations consistently identified the vertical support as a critical region experiencing elevated stress. Increasing its cross-sectional area was intended to improve resistance to bending, reduce deformation, and distribute the applied load more effectively.

The modified design will be evaluated using static stress analysis and mesh refinement to determine whether the additional material improves structural performance. The increase in mass will also be considered when comparing the three designs.

<img width="584" height="463" alt="Screenshot 2026-10-27 212257" src="https://github.com/user-attachments/assets/8bddd61b-6920-4a10-b2e8-e2874e28e2e3" />

Design III Stress and Displacement Analysis

<img width="1280" height="709" alt="Screenshot 2026-10-27 212936" src="https://github.com/user-attachments/assets/a4c60f96-1cc3-4ea8-a7ba-62373d35a497" />

<img width="1280" height="683" alt="Screenshot 2026-10-27 212950" src="https://github.com/user-attachments/assets/2eabde98-14d3-4ed4-a02d-2494e01d0fb1" />

Okay forget it it's still bending.

Design IV

For the fourth and FINAL design iteration, we will keep the extra-extruded vertical feature while adding on an isosceles triangle feature to connect all three figures together. 

<img width="843" height="602" alt="Screenshot 2026-10-27 213611" src="https://github.com/user-attachments/assets/e69b738d-393b-4f41-8377-599d6f50822d" />

<img width="1089" height="622" alt="Screenshot 2026-10-27 213628" src="https://github.com/user-attachments/assets/d74947eb-6746-4f52-ac14-1e8b0f8b45cd" />

<img width="790" height="515" alt="Screenshot 2026-10-27 213800" src="https://github.com/user-attachments/assets/29ec234d-3164-4b1d-99da-61dca5329dae" />

After reiterating the design with three more features (triangle support, fillet 1, and fillet 2), I re-ran the stress and displacement analysis. 

<img width="1280" height="677" alt="image" src="https://github.com/user-attachments/assets/dd1413bf-6968-4368-aae8-45025fb130fe" />

I believe the main factor of every design iteration not fulfilling the safety factor requirements is because of the material I used for the bracket (Aluminum 6061).

## Communicate

Preliminary Findings

The initial finite element simulations demonstrated that mesh refinement can significantly affect the calculated maximum stress. The maximum stress increased from 341.023 MPa to 451.690 MPa between the first two simulations, producing a 24.50% difference.

The initial safety factor of 0.806 was below the required value of 4, indicating that the original bracket did not meet the strength requirement under the preliminary simulation conditions.

These findings emphasize the importance of validating simulation results before using them to make design decisions. The remaining analysis will focus on verifying mesh convergence, improving the bracket geometry, and evaluating the tradeoffs between strength, stiffness, and mass.

Engineering Lessons Learned

One important lesson from this assignment was understanding how mesh size affects the accuracy of finite element analysis. Refining the mesh produced a significant change in the maximum stress, demonstrating that a single simulation may not provide sufficiently reliable results for design optimization.

I also learned that stress concentrations can develop where structural features connect, particularly when a relatively thin support transfers a large load between components. Examining these regions helps identify where geometric modifications may improve structural performance.

Another important consideration is the selection of boundary conditions. Fixed constraints simplify the simulation but may not fully represent the physical interaction between the bracket and the rigid T-beam. Understanding these assumptions is necessary when interpreting the results.

### MEGR 2157 LINK FEA

As part of the additional MEGR 2157 requirements, the separate link will undergo the same finite element analysis process. Three geometry iterations will be evaluated, with mesh convergence studies performed for each design.

# Objective

The objective of this assignment was to evaluate the structural performance of the linkage using Finite Element Analysis (FEA) in Autodesk Fusion 360. The analysis focused on determining maximum von Mises stress, total displacement, and minimum safety factor under an applied load of 2,891.34 N. The design was evaluated against a required safety factor of 2.0, and modifications were made to improve its structural performance.

# Analyze

## Initial FEA Analysis

<img width="1131" height="659" alt="Screenshot 2026-10-27 220502" src="https://github.com/user-attachments/assets/a5d28fbd-2722-4b4f-b0ee-8ad41a6e42ca" />

A static stress simulation was performed on the initial linkage design. A pin constraint was applied at the upper hole, and a downward bearing load of 2,891.34 N was applied to the lower hole.

The initial simulation produced the following results:

- Maximum von Mises stress: 141.407 MPa
- Maximum displacement: 0.819 mm
- Minimum safety factor: 1.945

The stress concentrations were primarily located around the lower hole where the bearing load was applied. The minimum safety factor of 1.945 was slightly below the required value of 2.0, indicating that the initial design did not meet the specified safety requirement.

<img width="1280" height="698" alt="Screenshot 2026-10-27 221345" src="https://github.com/user-attachments/assets/3ac77be0-59b8-4416-8125-05b4282e3641" />

<img width="1280" height="692" alt="Screenshot 2026-10-27 221403" src="https://github.com/user-attachments/assets/597ff57d-c3cf-46c0-a922-6f3a235676fe" />

<img width="1280" height="683" alt="Screenshot 2026-10-27 221435" src="https://github.com/user-attachments/assets/e6251072-e97f-4bf8-bd9b-7abbf32da644" />

## Design Iteration

After reviewing the initial FEA results, the linkage geometry was modified to improve the distribution of stress throughout the component. The revised design incorporated smoother, rounded transitions around the ends of the linkage.

The purpose of this modification was to reduce stress concentrations and improve the minimum safety factor without changing the applied loading conditions.

<img width="1280" height="703" alt="Screenshot 2026-10-27 222239" src="https://github.com/user-attachments/assets/50ac771b-64ef-45ad-aac3-ca2a1fed8a75" />

## Second FEA Analysis

A second static stress simulation was performed using the revised linkage geometry under the same applied load.

The second simulation produced the following results:

- Maximum von Mises stress: 110.409 MPa
- Maximum displacement: 4.241 mm
- Minimum safety factor: 2.491

The revised geometry reduced the maximum stress and increased the minimum safety factor above the required value of 2.0.

However, the maximum displacement increased significantly, indicating a reduction in overall stiffness or a change in deformation behavior. Further evaluation would be necessary to determine whether the displacement is acceptable for the intended application.

<img width="1280" height="714" alt="Screenshot 2026-10-27 222552" src="https://github.com/user-attachments/assets/7f401d00-581e-493a-a371-72bad94c42fd" />

<img width="1280" height="724" alt="Screenshot 2026-10-27 222652" src="https://github.com/user-attachments/assets/5fb92127-cd90-4c3f-89aa-abc418676025" />

<img width="1280" height="662" alt="Screenshot 2026-10-27 222702" src="https://github.com/user-attachments/assets/7469a0ed-e53b-42eb-99ec-57f7a7e85ff9" />

# Decide

Based on the simulation results, the revised linkage design was selected because it satisfied the required minimum safety factor of 2.0.

The redesign decreased maximum von Mises stress by approximately 21.92% and increased the minimum safety factor by approximately 28.07%.

Although the revised design performed better in terms of stress and safety factor, the increased displacement presents a potential concern. The revised design is therefore acceptable based on the safety factor requirement, pending verification of displacement limits and mesh convergence.

# Communicate

The FEA simulations demonstrated how relatively small geometric modifications can significantly affect the structural behavior of a mechanical component.

The initial design failed to meet the required safety factor, while the revised design achieved a minimum safety factor of 2.491.

The results also demonstrated the importance of evaluating multiple performance criteria. Although stress decreased and safety factor increased, the revised design experienced greater displacement.

## Lessons Learned

This assignment reinforced the importance of using FEA to identify stress concentrations and evaluate design modifications. I learned that improving one aspect of a design does not necessarily improve its overall performance, and that both strength and stiffness must be considered when evaluating a mechanical component.

Time Spent

The total time spent on this assignment was roughly four hours, dedicating the most time to the bracket analysis. Aluminum will be the death of me.

CAD Files

<https://a360.co/4d3vZLf>

