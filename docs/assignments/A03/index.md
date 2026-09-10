<!DOCTYPE html>
<html lang="en">

<head>


<!-- ===================================================== -->
<!-- TITLE -->
<!-- ===================================================== -->

<h1>Parametric and FEA Design</h1>

<p>
    <strong>Course:</strong> MEGR 2157
</p>

<p>
    <strong>Name:</strong> Kelsey Skipper
</p>

<p>
    <strong>Date:</strong> 9.9.26
</p>


<!-- ===================================================== -->
<!-- OBJECTIVE -->
<!-- ===================================================== -->

<h2>OBJECTIVE</h2>


<h3>Problem Statement</h3>

<p>
    The objective of this assignment was to design an aluminum bar subjected
    to direct tension while satisfying a maximum axial deflection requirement.
    The design was developed using analytical calculations, parametric CAD,
    and finite element analysis (FEA).
</p>


<div class="picture">

    <!-- INSERT ASSIGNMENT FIGURE -->

    <img src="images/assignment-figure.png"
         alt="Assignment figure">

    <p>
        Figure 1. Original assignment geometry and loading condition.
    </p>

</div>


<h3>Design Requirements</h3>

<p>
    The design requirements for the bar were:
</p>

<p>
    Applied load: 400 lbf
</p>

<p>
    Maximum axial deflection: 0.009 in
</p>

<p>
    Material: Aluminum
</p>

<p>
    Young's modulus: 8.5 × 10<sup>6</sup> to
    11.5 × 10<sup>6</sup> psi
</p>

<p>
    Required cross section: Circular
</p>

<p>
    Specified aluminum yield strength:
    40 ksi
</p>


<h3>Initial Design</h3>

<p>
    An aluminum 6061 bar with a diameter of 0.500 in was selected for the
    initial design. A Young's modulus of 10,000,000 psi was used for the
    analytical calculations.
</p>



<!-- ===================================================== -->
<!-- ANALYZE -->
<!-- ===================================================== -->

<h2>ANALYZE</h2>


<h3>Cross-Sectional Area</h3>

<p>
    The cross-sectional area of the circular bar was calculated using:
</p>

<div class="equation">

    A = πd² / 4

</div>

<div class="equation">

    A = π(0.500 in)² / 4

</div>

<div class="equation">

    A = 0.19635 in²

</div>


<div class="picture">

    <!-- INSERT CROSS SECTION SKETCH -->

    <img src="<img width="1025" height="634" alt="circlesketchA3" src="https://github.com/user-attachments/assets/1c72d264-ad5f-41b3-ba8d-3dbc7fb687aa" />
"
         alt="Circular cross section">

    <p>
        Figure 2. Circular cross section used for the bar.
    </p>

</div>


<h3>Axial Deflection</h3>

<p>
    The axial deflection of a bar subjected to direct tension is given by:
</p>

<div class="equation">

    δ = FL / AE

</div>

<p>
    Solving for the required length:
</p>

<div class="equation">

    L = δAE / F

</div>


<p>
    Substituting the selected values:
</p>

<div class="equation">

    L =
    (0.009 in)(0.19635 in²)(10,000,000 psi)
    / (400 lbf)

</div>

<div class="equation">

    L = 44.18 in

</div>


<p>
    Therefore, the analytical calculation determined that the bar should
    have a length of approximately <strong>44.18 in</strong>.
</p>


<div class="picture">

    <!-- INSERT HAND CALCULATION PICTURE -->

    <img src="<img width="1025" height="634" alt="image" src="https://github.com/user-attachments/assets/dc01ef1d-adfd-4598-8db1-84b9cd442822" />
"
         alt="Hand calculations">

    <p>
        Figure 3. Hand calculations for the initial design.
    </p>

</div>


<h3>Stress Analysis</h3>

<p>
    The nominal axial stress was calculated using:
</p>

<div class="equation">

    σ = F / A

</div>

<div class="equation">

    σ = 400 lbf / 0.19635 in²

</div>

<div class="equation">

    σ = 2037 psi

</div>

<div class="equation">

    σ = 2.04 ksi

</div>


<h3>Analytical Safety Factor</h3>

<p>
    Using the specified yield strength of 40 ksi:
</p>

<div class="equation">

    n = S<sub>y</sub> / σ

</div>

<div class="equation">

    n = 40 ksi / 2.04 ksi

</div>

<div class="equation">

    n ≈ 19.6

</div>


<h3>Parametric CAD Analysis</h3>

<p>
    The design was modeled parametrically in Autodesk Fusion. User
    parameters were created so that the geometry could automatically
    update when the loading or design requirements were changed.
</p>


<p>
    The parameters used were:
</p>

<p>
    <strong>Load:</strong> 400 lbf
</p>

<p>
    <strong>E:</strong> 10,000,000 psi
</p>

<p>
    <strong>MaxDeflection:</strong> 0.009 in
</p>

<p>
    <strong>Diameter:</strong> 0.500 in
</p>

<p>
    <strong>Area:</strong> PI*Diameter^2/4
</p>

<p>
    <strong>Length:</strong> MaxDeflection*Area*E/Load
</p>


<div class="picture">

    <!-- INSERT FUSION PARAMETER SCREENSHOT -->

    <img src="<img width="897" height="356" alt="Screenshot 2026-09-10 031456" src="https://github.com/user-attachments/assets/1397ff15-3249-4d14-91aa-5ae591274b97" />
"
         alt="Fusion parameters">

    <p>
        Figure 4. Parametric equations and user parameters in Fusion.
    </p>

</div>


<h3>Parametric Equation</h3>

<p>
    The length parameter was defined using the analytical deflection
    equation:
</p>

<div class="equation">

    Length = MaxDeflection × Area × E / Load

</div>


<p>
    This equation allows the bar length to automatically update based on
    the selected load, material stiffness, allowable deflection, and
    cross-sectional area.
</p>


<div class="picture">

    <!-- INSERT CAD MODEL -->

    <img src="<img width="1280" height="722" alt="extrudeA3" src="https://github.com/user-attachments/assets/f9321daa-180b-4e47-ba8d-f07eb5337649" />
"
         alt="Completed CAD model">

    <p>
        Figure 5. Completed parametric CAD model.
    </p>

</div>



<!-- ===================================================== -->
<!-- FEA ANALYSIS -->
<!-- ===================================================== -->

<h3>FEA Setup</h3>

<p>
    The completed CAD model was imported into the Fusion Simulation
    workspace. Aluminum 6061 was assigned as the material. The left end
    of the bar was fixed, and a 400 lbf tensile load was applied to the
    opposite end.
</p>


<div class="picture">

    <!-- INSERT MATERIAL SCREENSHOT -->

    <img src="<img width="701" height="316" alt="Screenshot 2026-09-10 031525" src="https://github.com/user-attachments/assets/8bb74101-2407-4984-800c-ae0f69890a03" />
"
         alt="Material assignment">

    <p>
        Figure 6. Aluminum 6061 material assignment.
    </p>

</div>


<div class="picture">

    <!-- INSERT FEA FIXTURE AND LOAD -->

    <img src="<img width="504" height="304" alt="Screenshot 2026-09-10 021935" src="https://github.com/user-attachments/assets/ab96f917-8a0f-4ddc-97f1-07cc3ed958f8"
         alt="FEA setup">
    <img src="<img width="792" height="476" alt="Screenshot 2026-09-10 022701" src="https://github.com/user-attachments/assets/fd06cffd-91ab-42ab-a8df-02fe35210e39"
         alt="FEA setup">

    <p>
        Figure 7. FEA fixture and loading conditions.
    </p>

</div>



<!-- ===================================================== -->
<!-- DECIDE -->
<!-- ===================================================== -->

<h2>DECIDE</h2>


<h3>Final Design</h3>

<p>
    Based on the analytical calculations and parametric CAD model, the
    selected design consisted of a 0.500 in diameter aluminum bar with a
    calculated length of 44.18 in.
</p>


<p>
    The analytical calculation predicted a maximum axial deflection of
    0.009 in, which satisfies the maximum allowable deflection requirement.
</p>


<h3>FEA Deflection</h3>

<div class="picture">

    <!-- INSERT FEA DEFLECTION MAP -->

    <img src="<img width="1280" height="752" alt="Screenshot 2026-09-10 030134" src="https://github.com/user-attachments/assets/6cf34b75-694e-43ac-9c75-1732c1074156"
         alt="FEA displacement map">

    <p>
        Figure 9. FEA axial displacement result.
    </p>

</div>


<p>
    Because the bar is aligned with the Y axis, the Y-direction displacement
    was used as the axial displacement.
</p>


<p>
    Hand calculation:
</p>

<div class="equation">

    δ<sub>hand</sub> = 0.009 in

</div>


<p>
    FEA result:
</p>

<div class="equation">

    δ<sub>FEA</sub> = [INSERT FEA VALUE] in

</div>


<h3>Percent Difference</h3>

<div class="equation">

    Percent Difference =
    |δ<sub>FEA</sub> − δ<sub>hand</sub>|
    / δ<sub>hand</sub> × 100%

</div>


<div class="equation">

    Percent Difference = [INSERT VALUE] %

</div>


<h3>Von Mises Stress</h3>

<div class="picture">

    <!-- INSERT VON MISES STRESS MAP -->

    <img src="<img width="1001" height="518" alt="Screenshot 2026-09-10 024911" src="https://github.com/user-attachments/assets/492990f5-3ff2-42b0-95e2-3f0517373b9c"
         alt="Von Mises stress map">

    <p>
        Figure 10. Von Mises stress distribution from FEA.
    </p>

</div>


<p>
    The maximum von Mises stress obtained from the simulation was:
</p>

<div class="equation">

    σ<sub>VM,max</sub> = [INSERT VALUE] ksi

</div>


<h3>FEA Safety Factor</h3>

<div class="equation">

    n = S<sub>y</sub> / σ<sub>VM,max</sub>

</div>

<div class="equation">

    n = 40 ksi / [INSERT STRESS]

</div>

<div class="equation">

    n = [INSERT SAFETY FACTOR]

</div>

<p>
    The estimated maximum stress was calculated using:
</p>

<div class="equation">

    σ<sub>max</sub> = K<sub>t</sub> σ<sub>nominal</sub>

</div>


<p>
    Nominal FEA stress:
    <strong>0.016</strong>
</p>

<p>
    Estimated maximum stress:
    <strong>2.04 ksi</strong>
</p>

<p>
    Estimated safety factor:
    <strong>19.6</strong>
</p>


<h3>Design Decision</h3>

<p>
    The final design was selected because it satisfies the required
    deflection constraint while maintaining a large margin against the
    specified yield strength.
</p>

<p>
    The results demonstrate that the design is primarily controlled by
    stiffness rather than strength. The cross-sectional area provides
    sufficient strength, while the required length is determined by the
    axial deflection requirement.
</p>



<!-- ===================================================== -->
<!-- COMMUNICATE -->
<!-- ===================================================== -->

<h2>COMMUNICATE</h2>


<h3>Results</h3>

<p>
    The analytical design produced a bar diameter of 0.500 in and a
    required length of 44.18 in. The theoretical axial deflection was
    0.009 in under a 400 lbf tensile load.
</p>


<p>
    The FEA results were compared with the analytical solution to verify
    the design.
</p>


<p>
    <strong>Hand calculation deflection:</strong>
    0.009 in
</p>

<p>
    <strong>FEA deflection:</strong>
    0.016
</p>

<p>
    <strong>Percent difference:</strong>
    77 %
</p>

<p>
    <strong>Maximum von Mises stress:</strong>
    26.363 MPa
</p>

<p>
    <strong>Safety factor:</strong>
    32.122
</p>


<h3>Comparison and Reflection</h3>

<p>
    The hand calculation and FEA results were compared to determine how
    closely the numerical simulation matched the analytical solution.
    The analytical equation assumes a uniform bar under direct axial
    loading, while FEA accounts for the actual CAD geometry, boundary
    conditions, material properties, and mesh.
</p>


<p>
    I'm not entirely sure why the percent difference seems so high comparing the hand calculations and measured calculations for the FEA stress, but it may have something to do with the Young's Modulus not being calculated correctly or the units not being correct even had being checked two or three times to be sure.
</p>


<p>
    For this design, the analytical solution provides a useful theoretical
    baseline because the bar is a simple member subjected to direct
    tension. The FEA simulation provides a numerical verification of the
    CAD model and loading conditions.
</p>


<h3>Lessons Learned</h3>

<p>
    This assignment demonstrated the relationship between analytical
    engineering calculations, parametric CAD, and FEA.
</p>


<p>
    One important lesson was that axial deflection depends directly on
    the applied load and bar length and inversely on the cross-sectional
    area and Young's modulus.
</p>


<div class="equation">

    δ = FL / AE

</div>


<p>
    Another lesson was the importance of using parametric CAD. By defining
    the length using an equation, the geometry can automatically respond
    to changes in the design parameters.
</p>


<p>
    FEA also demonstrated the importance of correctly interpreting
    displacement directions. Since the bar was aligned with the Y axis,
    the Y displacement represented the axial elongation.
</p>


<h3>Mistakes and Troubleshooting</h3>

<p>
    I had some issues essentially re-learning Fusion and making sure I had all the steps correct and in the right order to be able to do this assignment efficiently and effectively. One of my main issues was remembering where everything was and how to get to it.
</p>


<p>
    I fixed these problems by making notes on how to get to things, and eventually was able to get to everything very quickly.
</p>



<h3>Time Spent</h3>

<p>
    The total amount of time spent completing this assignment was:
    <strong>4 hours</strong>.
</p>



<!-- ===================================================== -->
<!-- CAD DOWNLOAD -->
<!-- ===================================================== -->

<h3>CAD File</h3>

<p>
    The completed CAD file can be accessed using the link below.
</p>


<p>

    <a href="(https://a360.co/4h0gN2D)">
        Download CAD File
    </a>

</p>


</body>

</html>
