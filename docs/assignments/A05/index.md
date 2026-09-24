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

Required section modulus:

`Z = SF(W)(LA) / (2Sy)`

`Z = (3.5)(1000)(2.4964) / [2(40,000)]`

`Z = 0.10922 in^3`

For a circular cross section:

`Z = πr^3 / 4`

Solving for radius:

`r = (4Z / π)^(1/3)`

`r = [4(0.10922) / π]^(1/3)`

`r = 0.518 in`

Therefore:

`d = 2r`

`d = 1.036 in`

**Feature A results:**

- `Z = 0.10922 in^3`
- `r = 0.518 in`
- `d = 1.036 in`

**Feature A — Stiffness**

For a cantilever beam with an end load:

`δA = FLA^3 / (3EI)`

For a circular section:

`I = πr^4 / 4`

`I = π(0.518)^4 / 4`

`I ≈ 0.0566 in^4`

Therefore:

`δA = (500)(2.4964)^3 / [3(9.99 × 10^6)(0.0566)]`

`δA ≈ 0.0092 in`

**Feature A final results:**

- `dA = 1.036 in`
- `δA ≈ 0.0092 in`

---

**Feature B — Axially Loaded Bar**

Feature B is modeled as an axially loaded member.

Known values:

- `P = 1000 lb`
- `LB = 1.400 in`
- `Sy = 40,000 psi`
- `SF = 3.5`
- `E = 9.99 × 10^6 psi`

**Feature B Free-Body Diagram**

<img width="416" height="310" alt="IMG_6725" src="https://github.com/user-attachments/assets/c81390cf-20d8-4ff7-854b-3325ef765831" />

**Feature B — Strength**

Axial stress is:

`σ = P / A`

Therefore:

`A = P / σ_allow`

`A = 1000 / 11,428.6`

`A = 0.0875 in^2`

Therefore, the minimum required cross-sectional area is:

`A_B = 0.0875 in^2`

For a rectangular section:

`A = bh`

Therefore:

`bh = 0.0875 in^2`

**Feature B — Stiffness**

Axial deformation is:

`δB = PLB / (AE)`

`δB = (1000)(1.4) / [(0.0875)(9.99 × 10^6)]`

`δB ≈ 0.00160 in`

**Feature B final results:**

- `AB = 0.0875 in^2 minimum`
- `δB ≈ 0.00160 in`

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

Maximum bending moment:

`Mmax = PL / 4`

`Mmax = (1000)(0.498) / 4`

`Mmax = 124.5 lb·in`

Required section modulus:

`Z = Mmax / σ_allow`

`Z = 124.5 / 11,428.6`

`Z = 0.01089 in^3`

For a rectangular cross section:

`Z = bh^2 / 6`

Therefore:

`bh^2 / 6 = 0.01089`

`bh^2 = 0.06536`

Therefore, the minimum Feature C strength requirement is:

`bh^2 = 0.06536`

**Feature C — Stiffness**

For a simply supported beam with a concentrated center load:

`δC = PLC^3 / (48EI)`

For a rectangular cross section:

`I = bh^3 / 12`

Therefore:

`δC = PLC^3 / (4Ebh^3)`

Substituting the known values:

`δC = (1000)(0.498)^3 / [4(9.99 × 10^6)bh^3]`

`δC = 1.552 × 10^-9 / (bh^3) in`

The supplied assignment material does not provide a numerical allowable-deflection value, so the final values of `bC` and `hC` cannot be uniquely determined from the available information.

The required strength relationship remains:

`bh^2 = 0.06536`

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
