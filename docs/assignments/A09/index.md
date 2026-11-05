# A9 – Pulleys
***Objective***

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

<img width="2234" height="1795" alt="IMG_7591" src="https://github.com/user-attachments/assets/d495a881-60bb-4889-b5c3-881d7dbda6a1" />

<img width="2203" height="1992" alt="IMG_7592" src="https://github.com/user-attachments/assets/bb722de1-ab3e-481f-8317-2cab5b2c5fbe" />

I first analyzed the forces acting on the belt. Using the initial tension and the assumed operating tension difference, I calculated a tight-side tension of 7.196 lbf and a loose-side tension of 2.804 lbf. These values gave a transmitted torque of 6.588 lbf·in.

The combined belt tensions were approximately 10 lbf, which I used as the radial load for my preliminary bearing analysis.

<img width="2498" height="4010" alt="IMG_7594" src="https://github.com/user-attachments/assets/14a3384a-1ab4-44e0-a960-92920d4c79ad" />

I then determined the required belt dimensions. I selected a 5/16-inch round polyurethane belt with a diameter of 0.3125 inches. The calculated maximum tensile stress was approximately 93.8 psi, giving a tensile factor of safety of 5.02.

Using an effective pulley diameter of 2.6875 inches and a center distance of 5 inches, I calculated a belt centerline circumference of approximately 18.44 inches.

The belt length and cross-section were used to create the belt geometry in Fusion 360. A final commercial belt selection would require confirming the available McMaster-Carr size and its installed tension.

<img width="1608" height="1258" alt="IMG_7593" src="https://github.com/user-attachments/assets/8113a66d-a6f0-4a98-8e1a-4c9adf843997" />

<img width="1278" height="623" alt="Screenshot 2026-11-04 175826" src="https://github.com/user-attachments/assets/06181d97-3b99-48bd-bedf-e3b1521c350c" />

I did the belt after the frame and the shafts, whoops!

Next, I calculated the minimum shaft diameter using AISI 1060 hardened steel. I used an assumed yield strength of 75,000 psi and a required factor of safety of 3.

The preliminary torsional calculation gave a minimum shaft diameter of approximately 0.1325 inches. I selected a nominal 3/8-inch shaft because it was larger than the calculated minimum and compatible with the selected journal bearings.

The actual shaft diameter in my Fusion 360 model was 0.37375 inches to provide clearance inside the bearing bore. The preliminary torsional factor of safety was approximately 68. This result does not include shaft bending, which would need to be evaluated for a complete strength analysis.

<img width="2655" height="4481" alt="IMG_7595" src="https://github.com/user-attachments/assets/5c43c555-5be9-4676-ba38-1e377f132139" />

<img width="1278" height="618" alt="Screenshot 2026-11-04 174337" src="https://github.com/user-attachments/assets/8b5e8756-b6e3-43cf-8f3a-11ef99b8c2be" />

I then analyzed the journal bearings. I selected oil-impregnated sintered bronze bearings with an inside diameter of 0.375 inches, an outside diameter of 0.500 inches, and a length of 0.250 inches.

Using an assumed radial load of 10 lbf per bearing, I calculated a bearing pressure of 106.67 psi, a shaft surface velocity of 147.26 ft/min, and a PV value of approximately 15,708 psi·ft/min.

These values were below the reference bearing limits used in my preliminary analysis. I selected sintered bronze because it is commonly used for lubricated rotating shaft applications. The final bearing specifications would need to be confirmed using the manufacturer's data.

<img width="1934" height="4814" alt="IMG_7598" src="https://github.com/user-attachments/assets/d8e557b0-39a7-41df-83fd-d44d47727636" />

<img width="890" height="430" alt="Screenshot 2026-11-04 182140" src="https://github.com/user-attachments/assets/67b21493-e27f-4016-84c9-dbe1d10a31f0" />

Finally, I designed the supporting frame using Aluminum 6061-T6. The frame was 7 inches long, 1.5 inches wide, and 0.5 inches thick. I added two raised bearing supports with 0.500-inch holes to hold the journal bearings.

The supports were positioned 5 inches apart to maintain the required shaft center distance.

<img width="1278" height="623" alt="Screenshot 2026-11-04 173842" src="https://github.com/user-attachments/assets/1748ac7e-2581-4544-bc5b-90ebbac271f2" />

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

<img width="1280" height="608" alt="Screenshot 2026-11-04 175341" src="https://github.com/user-attachments/assets/bb109cf3-ab31-44fd-87fc-4927fe8c6fdf" />

**Communicate**

I created the pulley system in Autodesk Fusion 360 using the dimensions and materials selected during my analysis.

I began by modeling the aluminum frame and adding two raised supports for the journal bearings. I positioned the supports 5 inches apart and created holes for the bearings.

I then modeled the two steel shafts and created the 3-inch-diameter pulleys. Each pulley was 0.500 inches thick and included a rounded groove for the polyurethane belt.

To create the belt, I sketched a closed path around both pulleys using two semicircular arcs and two straight sections. I positioned the belt path at the center of the pulley grooves and used the Sweep tool with a 0.3125-inch circular profile.

I modeled the journal bearings using concentric circles and extruded each bearing 0.250 inches into its support. I also extended both shafts into their bearings to represent their installed positions.

<img width="1273" height="619" alt="Screenshot 2026-11-04 175041" src="https://github.com/user-attachments/assets/2ee7f247-f586-471f-bdcc-781425b848e2" />

<img width="1280" height="686" alt="Screenshot 2026-11-04 181731" src="https://github.com/user-attachments/assets/442b9c34-6f97-4f1c-a452-c9c03be1e177" />

The completed model contains nine separate bodies: the frame, two shafts, two pulleys, the polyurethane belt, and two journal bearings.

<img width="231" height="516" alt="Screenshot 2026-11-04 182056" src="https://github.com/user-attachments/assets/595ca51d-2695-4e58-9956-e4b622b76445" />

I assigned materials and appearances to distinguish the different components and make the assembly easier to understand.

<img width="1280" height="620" alt="Screenshot 2026-11-04 182422" src="https://github.com/user-attachments/assets/a209acda-6a69-4053-9483-dc9a9716da7f" />

<img width="1278" height="623" alt="image" src="https://github.com/user-attachments/assets/e68c839b-edf8-47dd-be77-bf8b5aa1ba05" />

The final CAD model shows how the pulleys, belt, shafts, bearings, and supporting frame fit together. The calculations provided preliminary support for the component dimensions and material selections.

Final Cad Model Link: <https://a360.co/4zEsEv2>

**Lessons Learned**

Through this assignment, I learned how to apply belt tension, shaft stress, and journal bearing calculations to a mechanical design. I also gained a better understanding of how material selection and component dimensions affect the performance of a pulley system.

One of the more challenging parts was creating the polyurethane belt in Fusion 360. I had to make sure the belt path was positioned correctly inside the pulley grooves before using the Sweep tool.

I also learned how important it is to consider clearances between moving components, especially between the shafts and journal bearings.

This assignment helped me connect engineering calculations with CAD modeling and showed me how the individual components work together in a mechanical power transmission system.

Time Spent

In total, I spent about 4 hours working on this assignment. Mostly just from writing out all of the calculations and figuring out how the heck to offset the plane for the belt to sit on. This one was really fun!
