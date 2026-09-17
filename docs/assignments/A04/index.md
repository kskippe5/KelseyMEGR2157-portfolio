# A4 – Motor Mount

## Objective
The objective for this assignment is to design a motor mount for the specified Brush 24 V DC Gear Motor with a 99.5:1 planetary gearbox. The motor mount will attach to a rigid wall A and must support a force of P = 300 N acting at the motor shaft. The design will consist of two primary features: Feature 1, which supports the motor, and Feature 2, which attaches the mount to the rigid wall.

Both features will initially be approximated as cantilever beams and analyzed using beam bending equations. The design must have a safety factor of 3 against yielding and a maximum allowable deflection of 0.30mm. The final design will be modeled parametrically in CAD and will include the required motor and wall mounting holes. A fully dimensioned multiview engineering drawing will also be created from the final CAD model.

Initial Feature 2 dimensions of 20 mm × 10 mm resulted in a calculated bending stress of 10.8 MPa, exceeding the allowable stress of 6.667 MPa. The feature thickness was increased to 13 mm, reducing the calculated stress to 6.39 MPa and the deflection to approximately 0.076 mm. The revised dimensions satisfy both the stress and deflection requirements.

Inital Concept:
The motor mount will be designed as an approximately L-shaped bracket consisting of a horizontal motor-supporting feature and a vertical wall-supporting feature. The final design will incorporate structural features such as ribs or gussets to increase stiffness and reduce deflection.

## Analyze
The motor has a 6mm diameter shaft extending approximately 12mm from the mounting face. The shaft is subjected to a 300 N force. This force creates a bending moment on the motor mount.

<img width="306" height="194" alt="IMG_6336" src="https://github.com/user-attachments/assets/d3830f03-324b-4829-b2df-8b62c20e478d" />

This moment will be used as the applied loading condition for the simplified beam analysis.

The material used for this motor mount is ABS Plastic.

*E*= 2240.000 MPa
*Sy*= 20.000 MPa

Feature 1:

<img width="427" height="322" alt="IMG_6338" src="https://github.com/user-attachments/assets/09f79690-4e64-4f9d-835a-bf8570c85c5c" />

Feature 1 was modeled as a cantilever beam fixed at the wall. The force applied at the motor shaft produces a bending moment on the feature. This approximation allows the beam bending equations to be used to estimate the required cross-sectional geometry.

Feature 2:

<img width="575" height="336" alt="IMG_6339" src="https://github.com/user-attachments/assets/d2e8d064-61c9-4718-bc29-e9ce071a73af" />

Feature 2 was modeled as a cantilever beam fixed to rigid wall A. The applied motor loading produces a bending moment in the wall-mounted feature. The beam approximation was used to determine the required cross-sectional geometry based on both yield strength and deflection.

Final Dimensions:
**F1**: 30x15x15mm
**F2**: 40x20x14mm

<img width="3024" height="4032" alt="IMG_6333" src="https://github.com/user-attachments/assets/7b6e0bf9-8efc-469d-9f94-1a5c18699e45" />
<img width="4284" height="5712" alt="IMG_6334" src="https://github.com/user-attachments/assets/f20cf1ae-75b1-4b4e-87eb-3d1939906fd2" />
Entire handwritten documentation for reference; including all of the mistakes I made :)

## Decide

The calculated dimensions from the stress and deflection analyses were compared to determine the controlling design requirement. The final dimensions were selected to satisfy both the required safety factor of 3 and the maximum allowable deflection of 0.30 mm. Dimensions were then adjusted to practical values suitable for the final CAD model while maintaining the required structural performance.

To reduce deflection of the motor mount, structural ribs and/or gussets were incorporated into the design along with increasing the overall thickness of Feature 2. Increasing the section height increases the area moment of inertia according to

*I*= bh^3/12

Because the height is cubed, increasing the effective structural depth can significantly increase bending stiffness. The final design therefore uses additional material strategically in areas where bending stiffness is most important.

Motor mounting:
4 x M3

*Clearance holes*
∅3.4 mm

*Mounting circle*
∅18 mm

*Shaft clearance*
Motor shaft:
∅6 mm

## Communicate

<img width="1280" height="764" alt="Screenshot 2026-09-17 040049" src="https://github.com/user-attachments/assets/da698b94-4b1f-440f-9f19-151f412eef1c" />
The initial sketch for Feature 2.

<img width="1280" height="726" alt="Screenshot 2026-09-17 040414" src="https://github.com/user-attachments/assets/e9e5b69a-36e2-42bd-9db1-ad2b1b5f55c2" />
<img width="1280" height="764" alt="Screenshot 2026-09-17 041308" src="https://github.com/user-attachments/assets/b63dfa83-5323-4a8c-8d46-21ac242407ba" />
Extrusion of Feature 2, where I then put in the mounting holes.

<img width="1280" height="727" alt="Screenshot 2026-09-17 042022" src="https://github.com/user-attachments/assets/6725cb2c-7a1f-4fa8-b7a2-1593b7667fe2" />
Initial sketch of Feature 1 next to Feature 2.

<img width="1280" height="722" alt="Screenshot 2026-09-17 042151" src="https://github.com/user-attachments/assets/d2e4772e-8c76-4a06-8020-ccfb3ec92a4d" />
Extrusion and movement of Feature 1 to be coincident with Feature 2.

<img width="1280" height="726" alt="Screenshot 2026-09-17 042625" src="https://github.com/user-attachments/assets/728c45fe-21a6-43a4-baaa-c31c6e75fcce" />
<img width="1280" height="722" alt="Screenshot 2026-09-17 042717" src="https://github.com/user-attachments/assets/824f8303-597e-41e4-9281-95f8bcecfbea" />
Implementation of both shaft holes on Feature 1.

<img width="1280" height="722" alt="Screenshot 2026-09-17 042759" src="https://github.com/user-attachments/assets/2edec364-48de-4bdc-90de-d2c060808e09" />
<img width="1280" height="722" alt="Screenshot 2026-09-17 042810" src="https://github.com/user-attachments/assets/a95cd58a-571d-46c2-b143-968d54ee60fd" />
<img width="1280" height="722" alt="Screenshot 2026-09-17 042823" src="https://github.com/user-attachments/assets/86d1e0e6-9911-47ed-bb71-f35055e222b9" />
<img width="532" height="539" alt="Screenshot 2026-09-17 042848" src="https://github.com/user-attachments/assets/8af65b77-873f-48d4-91e1-475a3d6de743" />
All isometric views and an inside look at the mounting holes.

During the initial CAD model, the mounting-hole geometry was positioned too close to the edge of the feature. The geometry was revised to provide adequate material around the holes while maintaining the required ∅3.4mm clearance holes.

<img width="1280" height="722" alt="Screenshot 2026-09-17 042717" src="https://github.com/user-attachments/assets/574aaea1-e9f1-4ee4-8276-dad6f0f1ce02" />
Final CAD Model.

**Final stress:**
Feature 1: σmax​= 6.40 MPa
Feature 2: σmax​= 6.39 MPa

Allowable stress:
σallow= 6.67MPa

**Final factor of safety:**
N= 3

Requirement: N >= 3

**Final deflection:**
Feature 1: δ= 0.17mm
Feature 2: δ= 0.28mm

Requirement: δ <= 0.30mm

In total, this assigment took around 4 hours, mostly because I kept getting distracted. I skipped over the material requirement in the instructions and was setback a bit since I chose steel to begin with.

**Multiview Drawing**
<img width="830" height="592" alt="A4 CAD drawing" src="https://github.com/user-attachments/assets/7e6b5184-30b4-40fb-9a5c-2896fca841d2" />

**FINAL CAD LINK:** <https://a360.co/4yKYvcU> 

This assignment demonstrated how beam theory can be used to develop an initial structural design before creating a CAD model. The analysis showed the importance of both yield strength and deflection when determining the geometry of a component. In particular, the relationship between cross-sectional height and the area moment of inertia demonstrated why material can be strategically positioned to increase stiffness. The design process also demonstrated the importance of considering the dimensions of the actual hardware, including shaft clearance and mounting-hole locations. The final CAD model and engineering drawing required the analytical results to be translated into a manufacturable design while maintaining appropriate engineering drawing conventions.
