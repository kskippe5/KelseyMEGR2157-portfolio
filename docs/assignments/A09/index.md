# A9 – Pulleys
**Objective**

The objective of this assignment was to design a pulley system that transfers rotational power between two parallel shafts. The system needed to operate between 1000 and 2000 RPM, have a center distance between 4 and 6 inches, and maintain a static belt tension between 4 and 6 lbf. The design also required a polyurethane belt, properly sized shafts, journal bearings, and a supporting frame. The required factor of safety was 3.

I used engineering calculations to determine the appropriate dimensions and materials before creating the pulley system in Autodesk Fusion 360.

For my design, I selected two 3-inch-diameter pulleys with a center distance of 5 inches. I used an operating speed of 1500 RPM and an initial belt tension of 5 lbf.

**Analyze**

I began by identifying the known values and unknown values for the pulley system.

Known values:

- Pulley diameter: 3.000 in
- Center distance: 5.000 in
- Rotational speed: 1500 RPM
- Initial belt tension: 5 lbf
- Required factor of safety: 3
- Polyurethane yield strength: 3.25 MPa

Unknown values:

- Tight-side and loose-side belt tensions
- Required belt diameter and circumference
- Minimum shaft diameter
- Journal bearing pressure
- Shaft surface velocity
- Bearing PV value

[Insert handwritten knowns and unknowns here.]

[Insert handwritten pulley system free-body diagram here.]

I first analyzed the forces acting on the belt. Using the initial tension and the assumed operating tension difference, I calculated a tight-side tension of 7.196 lbf and a loose-side tension of 2.804 lbf. These values gave a transmitted torque of 6.588 lbf·in.

The combined belt tensions were approximately 10 lbf, which I used as the radial load for my preliminary bearing analysis.

[Insert handwritten belt tension and torque calculations here.]

I then determined the required belt dimensions. I selected a 5/16-inch round polyurethane belt with a diameter of 0.3125 inches. The calculated maximum tensile stress was approximately 93.8 psi, giving a tensile factor of safety of 5.02.

Using an effective pulley diameter of 2.6875 inches and a center distance of 5 inches, I calculated a belt centerline circumference of approximately 18.44 inches.

The belt length and cross-section were used to create the belt geometry in Fusion 360. A final commercial belt selection would require confirming the available McMaster-Carr size and its installed tension.

[Insert handwritten belt diameter, stress, factor of safety, and circumference calculations here.]

[Insert picture of belt path sketch in Fusion 360 here.]

Next, I calculated the minimum shaft diameter using AISI 1060 hardened steel. I used an assumed yield strength of 75,000 psi and a required factor of safety of 3.

The preliminary torsional calculation gave a minimum shaft diameter of approximately 0.1325 inches. I selected a nominal 3/8-inch shaft because it was larger than the calculated minimum and compatible with the selected journal bearings.

The actual shaft diameter in my Fusion 360 model was 0.37375 inches to provide clearance inside the bearing bore. The preliminary torsional factor of safety was approximately 68. This result does not include shaft bending, which would need to be evaluated for a complete strength analysis.

[Insert handwritten shaft diameter and factor of safety calculations here.]

[Insert picture of drive and driven shafts in Fusion 360 here.]

I then analyzed the journal bearings. I selected oil-impregnated sintered bronze bearings with an inside diameter of 0.375 inches, an outside diameter of 0.500 inches, and a length of 0.250 inches.

Using an assumed radial load of 10 lbf per bearing, I calculated a bearing pressure of 106.67 psi, a shaft surface velocity of 147.26 ft/min, and a PV value of approximately 15,708 psi·ft/min.

These values were below the reference bearing limits used in my preliminary analysis. I selected sintered bronze because it is commonly used for lubricated rotating shaft applications. The final bearing specifications would need to be confirmed using the manufacturer's data.

[Insert handwritten journal bearing pressure, velocity, and PV calculations here.]

[Insert picture of journal bearings in Fusion 360 here.]

Finally, I designed the supporting frame using Aluminum 6061-T6. The frame was 7 inches long, 1.5 inches wide, and 0.5 inches thick. I added two raised bearing supports with 0.500-inch holes to hold the journal bearings.

The supports were positioned 5 inches apart to maintain the required shaft center distance.

[Insert picture of frame dimensions in Fusion 360 here.]

**Decide**

After completing my calculations, I selected the final dimensions and materials for the pulley system.

My final design included:

- Two 3-inch-diameter AISI 1018 steel pulleys
- Two AISI 1060 hardened steel shafts with modeled diameters of 0.37375 inches
- One 5/16-inch round polyurethane belt
- Two SAE 841 oil-impregnated sintered bronze journal bearings
- One Aluminum 6061-T6 supporting frame
- A shaft center distance of 5 inches
- An operating speed of 1500 RPM

I selected identical pulleys to create a 1:1 speed ratio. This allows the driven pulley to rotate at approximately the same speed as the drive pulley, assuming no slipping.

I chose the polyurethane belt because its calculated tensile factor of safety exceeded the required value of 3. I selected the nominal 3/8-inch shafts because they exceeded the preliminary minimum diameter and fit the selected journal bearings.

The sintered bronze bearings were selected because the calculated pressure, velocity, and PV values were within the reference limits used in the analysis.

I chose Aluminum 6061-T6 for the supporting frame because it is lightweight, strong, and suitable for mechanical structures.

[Insert picture of selected materials and component dimensions here.]

**Communicate**

I created the pulley system in Autodesk Fusion 360 using the dimensions and materials selected during my analysis.

I began by modeling the aluminum frame and adding two raised supports for the journal bearings. I positioned the supports 5 inches apart and created holes for the bearings.

I then modeled the two steel shafts and created the 3-inch-diameter pulleys. Each pulley was 0.500 inches thick and included a rounded groove for the polyurethane belt.

To create the belt, I sketched a closed path around both pulleys using two semicircular arcs and two straight sections. I positioned the belt path at the center of the pulley grooves and used the Sweep tool with a 0.3125-inch circular profile.

I modeled the journal bearings using concentric circles and extruded each bearing 0.250 inches into its support. I also extended both shafts into their bearings to represent their installed positions.

[Insert picture of pulley and groove geometry here.]

[Insert picture of belt sweep in Fusion 360 here.]

[Insert picture of journal bearing installation here.]

The completed model contains nine separate bodies: the frame, two shafts, two pulleys, the polyurethane belt, and two journal bearings.

I assigned materials and appearances to distinguish the different components and make the assembly easier to understand.

[Insert picture of completed pulley system from an isometric view here.]

[Insert picture of completed pulley system from a top view here.]

The final CAD model shows how the pulleys, belt, shafts, bearings, and supporting frame fit together. The calculations provided preliminary support for the component dimensions and material selections.

**Lessons Learned**

Through this assignment, I learned how to apply belt tension, shaft stress, and journal bearing calculations to a mechanical design. I also gained a better understanding of how material selection and component dimensions affect the performance of a pulley system.

One of the more challenging parts was creating the polyurethane belt in Fusion 360. I had to make sure the belt path was positioned correctly inside the pulley grooves before using the Sweep tool.

I also learned how important it is to consider clearances between moving components, especially between the shafts and journal bearings.

This assignment helped me connect engineering calculations with CAD modeling and showed me how the individual components work together in a mechanical power transmission system.

Time Spent

