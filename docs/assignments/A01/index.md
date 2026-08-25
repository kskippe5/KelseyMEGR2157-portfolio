# KelseysMEGR2157-portfolio
This is my engineering design portfolio for Sophomore Design.

# A1 Engineering Portfolio

**Engineering is the art of making decisions you can defend.**

## Decide

### Homepage Identity

The homepage is the entry point for an employer, instructor, or engineering colleague evaluating this portfolio. It therefore needs to communicate immediately that the site is a record of mechanical engineering work rather than a personal website or conventional résumé. The homepage identifies the portfolio owner, establishes mechanical engineering as the technical focus, and explains that the work is organized around analysis, engineering decisions, and technical communication. This organization allows a reader to understand both the purpose of the portfolio and the standard used to document its contents before navigating to individual assignments. The homepage is intentionally concise because a professional reader should be able to determine the purpose and structure of the site without reading an extended personal biography.

### Intentional Customization

I changed the portfolio's accent color from the template default to a restrained dark-blue color scheme. This change was made to improve visual hierarchy and navigation rather than for aesthetic preference. A technical portfolio contains multiple types of information, including headings, navigation elements, figures, calculations, and explanatory text. A consistent accent color provides a visual distinction between navigation and technical content, allowing a reader to identify the site's organizational structure while scanning a page. The template's default color scheme did not provide the visual distinction I wanted between these elements, so the color was changed to better support rapid navigation through technical documentation.

### Documentation Standard

**Every assignment entry will state the governing model and its assumptions, document the criteria and reasoning behind significant decisions, and provide sufficient calculations, figures, and supporting evidence for another engineering student to reproduce the work without requesting additional information.**


# Analyze

## Task A: Portfolio Analysis

### Portfolio 1: Justice Nyazika

The first portfolio analyzed was Justice Nyazika's mechanical engineering portfolio, hosted through GitHub Pages. The portfolio organizes information into sections including About, Skills, Projects, Certifications, Journey, Resume, and Contact. The Projects section provides examples of engineering work involving mechanical design, robotics, engines, shock absorbers, vehicles, and Arduino-based systems.

#### Navigability

The portfolio provides a direct navigation structure that separates projects and professional information into identifiable sections. A reader looking for a particular project can access the Projects section without navigating through a continuous résumé-style document. This organization is effective for a recruiter who needs to identify the author's areas of experience quickly. However, the project summaries do not all provide the same level of internal organization, so a reader seeking detailed technical evidence may need to inspect multiple sections or pages to determine how a particular project was completed.

#### Reproducibility

The portfolio provides enough information to identify the general purpose and subject of several projects, but it does not consistently provide the dimensions, input conditions, assumptions, calculations, fabrication procedures, testing conditions, or design files required for another engineer to reproduce the work independently. The portfolio therefore functions primarily as a professional overview rather than a complete engineering record. A colleague could understand what type of work was performed, but could not necessarily reconstruct the design or analysis without additional information from the author.

#### Evidence of Reasoning

The portfolio primarily emphasizes completed projects, skills, and outcomes. It provides less evidence of the alternatives considered before the final designs were selected. Information about design iterations, decision criteria, failed approaches, or quantitative tradeoffs would make the engineering reasoning more visible. This is an important distinction between documenting a project as an accomplishment and documenting it as an engineering decision process.

#### Professional Tone

The portfolio uses technical terminology associated with mechanical engineering and engineering technology, including CAD, FEA, CFD, Arduino, Python, and product development. The descriptions are generally oriented toward engineering experience rather than personal interests. However, some descriptions emphasize broad project claims rather than measurable engineering results. The tone is appropriate for an engineering portfolio, but the technical documentation could be strengthened by consistently identifying requirements, methods, results, and evidence.


### Portfolio 2: Nhan Dang

The second portfolio analyzed was Nhan Dang's mechanical engineering portfolio. The portfolio focuses on mechanical design, CAD modeling, robotics, prototyping, fabrication, testing, and technical documentation. Its project-oriented structure is particularly relevant to the purpose of this course because it presents engineering work as a process rather than only as a collection of completed products.

#### Navigability

The portfolio separates technical projects from general professional information, allowing a reader to locate engineering work without navigating through unrelated material. Individual projects are presented as distinct pieces of work, which allows an employer to select an area of interest and examine it independently. This structure is effective for a technical reader because the navigation corresponds to the way an engineer would typically review a project portfolio: identify a project, inspect the design, and then examine the supporting technical information.

#### Reproducibility

The portfolio provides more evidence of the engineering process than a résumé-only portfolio. Its descriptions identify activities such as mechanical layout, CAD development, prototyping, fabrication, testing, and documentation. These categories provide a reader with information about how the work progressed from a concept toward a physical result. However, reproducibility still depends on the amount of quantitative information provided for each individual project. Dimensions, material specifications, calculations, tolerances, and test conditions would further increase the ability of another engineer to reproduce the work.

#### Evidence of Reasoning

This portfolio provides stronger evidence of engineering reasoning because it presents projects through their design and development processes rather than only listing finished results. References to mechanical layout, interfaces, prototyping, fabrication, testing, and revisions allow the reader to infer how the final design developed. The portfolio could provide even stronger evidence by explicitly documenting rejected alternatives and the criteria used to select the final design.

#### Professional Tone

The language is concise and technically oriented. The descriptions focus on engineering activities such as mechanical design, CAD, fabrication, testing, and sensor integration rather than relying on general statements about being interested in engineering. This makes the content appropriate for a technical audience, including engineering employers and collaborators. The writing could be strengthened further through additional quantitative results, but the existing tone is appropriate for a professional engineering record.

### Portfolio Comparison

The two portfolios demonstrate different priorities in engineering documentation. Justice Nyazika's portfolio functions primarily as a professional overview that allows a reader to identify skills and project experience quickly. Nhan Dang's portfolio places greater emphasis on the engineering process, including design, fabrication, testing, and technical documentation. For this portfolio, I will prioritize the second approach because the purpose of an engineering record is not only to demonstrate what was produced but also to provide evidence of how the problem was analyzed, how alternatives were evaluated, and why the final decision was selected.


# Task B: Product Analysis

## Product: Spring-Loaded Wooden Clothespin

### Primary Function

The primary function of the clothespin is to generate and maintain a compressive clamping force between two opposing jaws in order to retain fabric against a supporting clothesline. The device converts the elastic deformation of a spring into a mechanical gripping force at the jaw surfaces.

### Governing Mechanical Model

The primary mechanical behavior of the clothespin can be modeled as a lever system subjected to moment equilibrium about the spring/pivot region.

The governing equilibrium relationship can be represented as:

$$
\sum M_O = 0
$$

For a simplified two-force representation, the relationship between spring force and clamping force can be expressed as:

$$
F_s d_s = F_c d_c
$$

where:

* $F_s$ = effective spring force
* $d_s$ = moment arm of the spring force about the pivot
* $F_c$ = clamping force at the jaw
* $d_c$ = moment arm from the pivot to the jaw contact point

This model explains how the spring-generated force is converted into the clamping force at the jaws. Because the jaw members rotate about the pivot region, the location of the spring force and the location of the fabric contact determine the resulting mechanical advantage.

The ability of the clothespin to retain fabric also depends on friction between the jaw surfaces and the fabric. The maximum idealized friction force can be represented as:

$$
F_f = \mu N
$$

where $F_f$ is the available friction force, $\mu$ is the coefficient of friction between the contacting surfaces, and $N$ is the normal clamping force.

### Model Assumption

The clothespin can be modeled as a rigid-body lever mechanism with negligible deformation of the jaw members relative to the rotation produced by the spring. This assumption is reasonable because the primary motion of the device occurs through rotation of the two jaw members, while the plastic components are substantially stiffer than the spring mechanism during normal operation.


## Component 1: First Plastic Jaw

<img width="1512" height="1512" alt="IMG_5835" src="https://github.com/user-attachments/assets/a1e6d345-b467-4bc8-80bd-43712259353a" />

The first member forms one half of the clothespin's lever mechanism. Its elongated geometry provides a handle region that allows the user to apply force away from the pivot while its opposite end forms one of the gripping surfaces. The distance between the gripping surface and the pivot determines the moment arm through which the clamping force acts. The distance between the user's applied force and the pivot similarly determines the mechanical advantage available when opening the clothespin. The relatively broad gripping region distributes the contact force over the fabric or material being held rather than concentrating the entire load at a single point.


## Component 2: Second Plastic Jaw

<img width="1512" height="1512" alt="IMG_5836" src="https://github.com/user-attachments/assets/669ae343-5710-4437-b637-da6158d47702" />

The second member forms the opposing jaw and works with the first member to create the clamping interface. Its geometry is approximately complementary to the first jaw so that the two members can rotate toward one another while maintaining a defined gripping region. The handle portion provides a location for the user to apply an opening force, while the jaw portion transfers the spring-generated force to the fabric. The alignment of the two members is important because misalignment would reduce the effective contact area and could cause the fabric to slip.


## Component 3: Wire Spring

<img width="1512" height="1512" alt="IMG_5837" src="https://github.com/user-attachments/assets/3aeeef34-9e6e-4f70-8c02-490c69ee0e98" />

The wire spring provides the elastic restoring force that biases the two plastic members toward the closed position. Its coiled geometry allows the spring to store elastic energy as the handles are squeezed apart. When the applied opening force is removed, the spring generates a restoring torque that rotates the plastic members back toward one another. The spring therefore performs two mechanical functions: it provides the force necessary for clamping and establishes the preferred closed position of the mechanism. The spring's location near the pivot also allows its force to produce a relatively large moment on the wooden members.


# Patent Research

The product analyzed is based on the conventional spring-loaded clothespin mechanism. One relevant patent is **U.S. Patent No. 2,471,606, "Clothespin," by Bruce Burns**. The patent describes a clothespin consisting of opposed members forming jaw and handle portions, with a spring arranged to urge the jaw portions toward one another.

The patent is relevant to the physical product because the mechanical architecture described in the patent corresponds to the three-component arrangement examined here: two opposing members and an elastic spring mechanism.

### Alternative Solutions

Several alternative mechanisms can perform the same primary engineering function of retaining fabric on a supporting line.

**1. One-piece spring clothespin:** Some clothespin designs use a single piece of resilient material whose geometry creates the spring action. This eliminates the separate coil spring and reduces the number of components.

**2. Push-on clothespin:** Another design uses geometry that allows the user to push the device directly onto the clothesline and fabric. Instead of relying on conventional handles that must be squeezed together, the user applies force by pushing the mechanism onto the supporting line.

**3. Binder clip:** A binder clip provides another mechanically different solution to the same general function of clamping material. Its sheet-metal arms and torsional spring generate a clamping force at opposing jaws.

### Design Decision

One significant design decision in the conventional clothespin is the use of a separate coil spring positioned between two opposing wooden members. This configuration separates the functions of the structural jaw members and the elastic force-producing element. The plastic components can therefore be shaped primarily to provide a comfortable handle and appropriate gripping geometry, while the spring supplies the restoring force required for clamping. Positioning the spring near the pivot also allows its force to generate a torque on the two members without requiring the spring to span the entire length of the device.

This configuration also allows the user to open the jaws by applying a relatively small force at the ends of the handles. The handle length creates a moment arm that provides mechanical advantage relative to the jaw contact region. The design therefore uses geometry to make a spring-generated clamping force controllable by a human operator.


# Communicate

### What Does It Mean to Defend an Engineering Decision; and Do I Currently Know How to Do It?

To defend an engineering decision means being able to explain not only what was chosen, but why that choice was appropriate given the requirements, constraints, available alternatives, and governing engineering principles. A defensible decision should be supported by evidence rather than preference. At the beginning of this semester, I understand the basic concept of defending a decision, but I do not yet consider myself fully proficient at doing it. I can explain the reasoning behind many of my choices, but I am still developing the ability to document that reasoning systematically through explicit criteria, quantitative comparisons, assumptions, and supporting evidence. My goal for this semester is to make my engineering decisions increasingly reproducible: another engineer should be able to examine my work and understand the reasoning well enough to agree with the decision, identify a limitation, or propose a better alternative.

### Time Spent

I spent approximately 5 hours on this assignment, including researching engineering portfolios, analyzing the selected mechanical product, researching its patent history, developing the portfolio site, documenting design decisions, and preparing the final engineering analysis.
