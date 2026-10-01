# A6 – [Topic]

## Objective
The objective of this project is to develop a parametric CAD model and detailed engineering drawing of the assigned bracket while applying engineering analysis to verify that the design satisfies the required strength and stiffness requirements. The bracket must be modeled so that its important dimensions and geometric features can be modified parametrically while maintaining the intended design relationships.

The design is evaluated using Aluminum 6061 as the selected material. The analysis considers the geometry of the linkage, applied loading, material strength, and stiffness. The final design will be communicated through the completed CAD model, engineering drawing, supporting calculations, and stress and stiffness sketches.
## Analyze
The bracket was analyzed by first identifying the important dimensions and loading relationships within the linkage. The primary geometry used for the analysis includes:

lA = 2.4964 in
lB = 1.400 in upward and 1.036 in horizontal
lC = 0.498 in

The selected material for the bracket is Aluminum 6061. The material properties used for the engineering analysis are

Yield strength: Sy = 40,000 psi
Elastic modulus: E = 68.9 GPa

The geometry and loading were considered using the linkage configuration provided for the assignment. The linkage section was analyzed using the requirements provided in Appendix E. The dimensions of the individual members and their orientations were used to establish the loading and reaction relationships acting on the bracket.

__Stress Analysis__

The bracket must withstand the forces transmitted through the linkage without exceeding the allowable stress of the selected material. The relevant loading conditions were identified from the linkage geometry and represented using free-body diagrams and multiview sketches.

The basic normal-stress relationship is

σ = F/A

where

σ = normal stress
F = applied force
A = cross-sectional area

For regions subjected to shear, the average shear stress can be calculated using

τ = V/A

where

τ = average shear stress
V = shear force
A = shear area

<img width="921" height="403" alt="IMG_6715" src="https://github.com/user-attachments/assets/2d594029-7808-4b68-b315-8fd6f89cab13" />

The stress calculations were used to identify areas of the bracket that experience the greatest loading. Particular attention was given to the connection regions and areas where the geometry changes, since these locations can experience higher stresses.

The material yield strength of \(40,000\ psi\) provides the strength limit used when evaluating the design. The calculated stresses must remain below the allowable stress for the design to be acceptable.

Stiffness Analysis

In addition to strength, the bracket was evaluated for stiffness. A bracket can have stresses below the material yield strength and still experience excessive deformation, so both requirements must be considered.

The stiffness behavior is related to the elastic modulus

E = σ/ϵ

where
E = elastic modulus
ϵ = strain
σ = normal stress

For Aluminum 6061

E = 68.9 GPa

The stiffness analysis was represented using multiview sketches to show how the bracket and linkage respond to the applied loading. These sketches help communicate the expected deformation direction and identify the portions of the geometry that contribute most strongly to the overall stiffness.

The stiffness evaluation was considered in both the vertical and horizontal directions because the linkage contains both vertical and horizontal components. The lB dimensions of 1.400 upward and 1.036 horizontally were therefore included when establishing the geometry used for the analysis.

__Parametric CAD Model__


<img width="401" height="230" alt="Screenshot 2026-09-24 041855" src="https://github.com/user-attachments/assets/7e5625c5-7368-42ab-8956-a938187c6071" />

After establishing the engineering requirements, the bracket was modeled parametrically in CAD. The purpose of the parametric model is to ensure that important dimensions can be changed without rebuilding the entire model.

The primary sketches were fully dimensioned and constrained so that the geometry remained consistent when dimensions were modified. Features such as holes, extrusions, fillets, and other geometric details were incorporated into the model based on the assigned bracket design.

The parametric approach also makes the model easier to revise if the stress or stiffness analysis indicates that a geometric change is necessary.

<https://a360.co/4d3vZLf>

__Engineering Drawing__

The final CAD model was used to create a detailed engineering drawing. The drawing communicates the dimensions and manufacturing information necessary to reproduce the bracket.

The drawing includes the appropriate multiview representation of the part, dimensions for critical features, and other required drawing information. The views were selected to clearly communicate the geometry without relying on a three-dimensional model alone.

The stress and stiffness multiview sketches provide additional engineering communication by showing how the bracket is expected to behave under loading.

<https://a360.co/46TAEfa>

## Decide
Aluminum 6061 was retained as the bracket material because its mechanical properties provide an appropriate combination of strength, stiffness, low density, and manufacturability for the design.

The final bracket geometry was developed to satisfy the required linkage dimensions while maintaining a practical and manufacturable shape. The parametric approach was selected because it allows the design to be modified efficiently if additional analysis identifies a need for increased strength or stiffness.

The critical dimensions were incorporated into the CAD model so that the linkage geometry remains consistent. The geometry associated with lA, lB, and lC was maintained as part of the overall design.

The stress analysis provides a method for checking whether the bracket can withstand the applied loading without yielding, while the stiffness analysis provides a method for checking whether deformation remains acceptable. Both analyses are necessary because a design that satisfies only the strength requirement may still have excessive deflection.

The final design therefore combines the required geometry, Aluminum 6061 material properties, strength considerations, stiffness considerations, and manufacturability into one parametric bracket model.

## Communicate
This project taught me how to develop a parametric bracket while considering both strength and stiffness. I learned how material selection, critical dimensions, and tolerances affect the design and manufacturing process. I also gained experience creating an engineering drawing that clearly communicates the design using dimensions, tolerances, material specifications, and standard drawing conventions.

The completed bracket design is communicated through the parametric CAD model, engineering drawing, calculations, and supporting sketches.

This assignment took me roughly two and a half hours to do, since I already had most of the calculations done really early on.

Final CAD model: <https://a360.co/4d3vZLf>
Final Drawing File: <https://a360.co/46TAEfa>
