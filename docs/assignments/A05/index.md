# Objective

The objective of this assignment is to design a bracket that attaches to a rigid T-beam and supports the required polyester strap loading. The bracket is divided into Features A, B, and C so that each feature can be analyzed using an appropriate mechanical model. Feature A is modeled as a cantilever beam, Feature B as an axially loaded member, and Feature C as a simply supported beam with a concentrated center load.

The bracket and linkage are designed using 6061 aluminum. The design must satisfy the required strength using a safety factor of 3.5. Appendix E also requires a linkage connecting Feature A to another cylindrical feature while carrying the same force. The Feature A connection requires a running/sliding fit, while the 1-in shaft connection requires a light assembly pressure fit.

Given:

- Applied force: `F = 500 lb`
- Total strap load: `W = 2F = 1000 lb`
- Safety factor: `SF = 3.5`
- Yield strength: `Sy = 40,000 psi`
- Elastic modulus: `E = 68.9 GPa`

Convert the elastic modulus to psi:

`E = (68.9 GPa)(145,038 psi/GPa)`

`E ≈ 9.99 × 10^6 psi`

Allowable stress:

`σ_allow = Sy / SF`

`σ_allow = 40,000 / 3.5`

`σ_allow = 11,428.6 psi`

---

# Analyze

**Feature A — Cantilever Beam**

Feature A is modeled as a cantilever beam.

<img width="578" height="293" alt="Screenshot 2026-09-24 035117" src="https://github.com/user-attachments/assets/b81e5e80-3bfa-40d9-a323-d7a65166df61" />

Known values:

- `F = 500 lb`
- `W = 1000 lb`
- `LA = 2.4964 in`
- `Sy = 40,000 psi`
- `SF = 3.5`
- `E = 9.99 × 10^6 psi`

Assumptions:

- Feature A behaves as a cantilever beam.
- Loading is static.
- The material remains elastic.
- Maximum bending stress occurs at the fixed end.
- The cross section is circular.
- The safety factor is applied to the yield strength.

**Feature A Free-Body Diagram**

<img width="465" height="255" alt="IMG_6723" src="https://github.com/user-attachments/assets/fa233865-8360-4322-a7bb-7c096da5c554" />

**Feature A — Strength**

<img width="921" height="403" alt="IMG_6715" src="https://github.com/user-attachments/assets/1fcdfe2a-6fa9-4052-9bd7-1e962ac6ca37" />

Strength calculations for Feature A

**Feature A — Stiffness**

<img width="337" height="369" alt="IMG_6719" src="https://github.com/user-attachments/assets/bc79207d-01b4-42e3-ae41-71313c87b30c" />

Stress calculations for Feature A
---

**Feature B — Axially Loaded Bar**

Feature B is modeled as an axially loaded member.

<img width="401" height="230" alt="Screenshot 2026-09-24 041855" src="https://github.com/user-attachments/assets/e87ea198-1e25-4354-ae6e-ba9794a94d6d" />

Known values:

- `P = 1000 lb`
- `LB = 1.400 in`
- `Sy = 40,000 psi`
- `SF = 3.5`
- `E = 9.99 × 10^6 psi`

**Feature B Free-Body Diagram**

<img width="416" height="310" alt="IMG_6725" src="https://github.com/user-attachments/assets/c81390cf-20d8-4ff7-854b-3325ef765831" />

**Feature B — Strength**

<img width="831" height="180" alt="IMG_6716" src="https://github.com/user-attachments/assets/7422ef8a-2655-4353-ab94-bdd8cd387b76" />

Teeny calculations for strength of Feature B

**Feature B — Stiffness**

<img width="327" height="180" alt="IMG_6720" src="https://github.com/user-attachments/assets/3a42943b-9fcb-4944-8b32-dafa2d8a77d1" />

More teeny calculations for stress of Feature B

---

**Feature C — Simply Supported Beam**

Feature C is modeled as a simply supported beam with a concentrated load at the center.

Known values:

- `P = 1000 lb`
- `LC = 0.498 in`
- `Sy = 40,000 psi`
- `SF = 3.5`

Assumptions:

- Feature C is simply supported.
- The load acts at the center.
- The cross section is rectangular.
- Loading is static.
- The material remains elastic.

**Feature C Free-Body Diagram**

<img width="380" height="248" alt="IMG_6724" src="https://github.com/user-attachments/assets/572a46de-4c79-414b-9c59-882ac8c60508" />

Because the load is centered:

`RA = RB = P / 2`

`RA = RB = 1000 / 2`

`RA = RB = 500 lb`

**Feature C — Strength**

<img width="715" height="331" alt="IMG_6717" src="https://github.com/user-attachments/assets/227376cd-1bbe-4228-a13f-2f59e9480cbf" />

Strength calculations for Feature C

**Feature C — Stiffness**

<img width="330" height="376" alt="IMG_6721" src="https://github.com/user-attachments/assets/e9dcdbbb-501b-4b2a-8c4f-8c0527cf8da5" />

The supplied assignment material does not provide a numerical allowable-deflection value, so the final values of `bC` and `hC` cannot be uniquely determined from the available information.

The required strength relationship remains:

bh^2 = 0.06536

---

**Appendix E — Linkage and Fits**

The linkage connects Feature A to another cylindrical feature and carries the same applied force. The selected linkage material is 6061 aluminum.

Linkage requirements:

- Material: `6061 Aluminum`
- Applied force: `500 lb`
- Feature A connection: running/sliding fit
- 1-in shaft connection: light assembly pressure fit

**Feature A linkage connection**

The calculated Feature A diameter is:

`dA = 1.036 in`

The provided running/sliding fit table places 1.036 in in the 0.71–1.19 in nominal-size range.

Using the RC2 values from the provided table:

Hole tolerance:

`+0.0005 / -0.0000 in`

Therefore:

`DA,hole = 1.0360 to 1.0365 in`

The corresponding clearance range is:

`0.0003 to 0.0012 in`

Therefore, the Feature A connection is designed as a running/sliding fit.

**1-in shaft connection**

The second cylindrical feature has:

`Dshaft = 1.000 in`

The required fit is:

`Light assembly pressure fit`

The supplied fit table is the running/sliding-fit table, so its RC2 clearance values are not used for this connection. The 1-in shaft remains a 1.000-in nominal shaft, with the final interference tolerance determined by the applicable pressure-fit specification.

**Summary of analytical results**

| Parameter | Result |
|---|---:|
| Material | 6061 Aluminum |
| Applied force | 500 lb |
| Total strap load | 1000 lb |
| Safety factor | 3.5 |
| Yield strength | 40,000 psi |
| Allowable stress | 11,428.6 psi |
| Elastic modulus | 9.99 × 10^6 psi |
| Feature A length | 2.4964 in |
| Feature A section modulus | 0.10922 in^3 |
| Feature A radius | 0.518 in |
| Feature A diameter | 1.036 in |
| Feature A deflection | ≈0.0092 in |
| Feature B length | 1.400 in |
| Feature B minimum area | 0.0875 in^2 |
| Feature B deflection | ≈0.00160 in |
| Feature C length | 0.498 in |
| Feature C reactions | 500 lb each |
| Feature C maximum moment | 124.5 lb·in |
| Feature C minimum section modulus | 0.01089 in^3 |
| Feature C strength equation | bh^2 = 0.06536 |
| Feature A linkage fit | RC2 running/sliding |
| Feature A linkage hole | 1.0360–1.0365 in |
| 1-in shaft | 1.000 in nominal |
| 1-in shaft fit | Light assembly pressure fit |

---

# Decide

The analytical calculations establish the minimum dimensions required for the bracket features and provide the starting dimensions for the CAD model.

Feature A requires a minimum radius of:

`rA = 0.518 in`

and therefore a minimum diameter of:

`dA = 1.036 in`

The calculated Feature A deflection is approximately:

`δA = 0.0092 in`

Feature B requires a minimum cross-sectional area of:

`AB = 0.0875 in^2`

with an estimated axial deformation of:

`δB = 0.00160 in`

Feature C requires a minimum section modulus of:

`ZC = 0.01089 in^3`

or:

`bChC^2 = 0.06536`

The final Feature C dimensions must satisfy both strength and stiffness requirements.

The linkage will be made from 6061 aluminum. Its Feature A connection will use the calculated 1.036-in Feature A diameter with a running/sliding RC2 fit. The linkage's second connection will accommodate the 1-in shaft using the required light assembly pressure fit.

---

# Communicate

**Final CAD Model**

<https://a360.co/4d3vZLf>

**Final important dimensions**

`dA = 1.036 in`

`AB ≥ 0.0875 in^2`

`ZC ≥ 0.01089 in^3`

`bChC^2 ≥ 0.06536`

`DA,hole = 1.0360–1.0365 in`

`Dshaft = 1.000 in nominal`

**Lessons Learned**

This assignment demonstrated how different portions of a mechanical component can be analyzed using different engineering models. Feature A was modeled as a cantilever beam, Feature B as an axially loaded member, and Feature C as a simply supported beam with a concentrated center load. Strength calculations were used to determine minimum dimensions, while stiffness calculations were used to evaluate deformation. The linkage analysis also demonstrated the importance of selecting appropriate fits and tolerances when connecting mechanical components. The analytical results were then used to make defensible design decisions and communicate the final design through CAD and engineering drawings.

**Total Time**
This assignment took me about 4 hours to do, which included bumps in the road and creating the CAD file. I'm going to sleep.
