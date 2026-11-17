# A10 – Lead Screw Translating System

## Objective
* This assignment was a group assignment that consisted of coordinating with teammates in order to design a project with set constraints. A tensile tester is a mechanism that through uniaxial tension allows engineers to test materials and gather information about it's properties such as yield strength, ultimate yield strength and elongation at break. This information can be used for deciding material usage in different applications. The objective of this assignment was to design a tensile tester that could handle a 2kN axial load and a crosshead speed from 1-50 mm/min. As a team we developed a lead screw, and ensure that our tensile tester would be accurate and could repeatedly apply a 2 kN load.
## Analyze
### Diameter- Farima Pournia 
* For deciding on what lead screw to select the diameter was first calculated. This was done by using the guidelines given like yield strength, force, and safety factor. The safety factor equation was used to be set equal to the stress equation which used the area of a circle for it's area equation. The parameters were then plugged into this equation and the diameter was solved for.
  <img width="1972" height="1484" alt="image" src="https://github.com/user-attachments/assets/354bc6d8-2f56-4bd2-b384-3b70e97cf214" />
* To select a diameter for the lead screw the closest diameter to the one calculated is 5.97 mm which corelates with a 3/8-10 screw. 
### Rotational Speed- Farima Pournia 
* The rotational speed of the lead screw was then calculated through the speed range given and the screw lead that was found through the diameter that was calculated. Using the equation for linear speed rotational speed was solved for. This equation was then used to plug in the lower and upper bounds of the linear speed range and a range for rotational speed was calculated.
 <img width="1848" height="784" alt="image" src="https://github.com/user-attachments/assets/09b3b669-2147-4408-8a6a-6c2f6bd9368c" />
 
### Torque Farima Pournia
* The next parameter that was calculated was torque by using the equation for a square threaded lead screw. The diameter of the actual screw selected was used and not the diameter that was calculated. The screw lead was found through the diameter of the screw selected and the coefficient of friction was found in the Machinery Handbook under the value for friction of steel against bronze. These values were plugged into the torque equation and solved.
  <img width="2084" height="1036" alt="image" src="https://github.com/user-attachments/assets/df96592f-498d-469c-ab97-d1d0d48b285d" />
* From calculating these parameters a lead screw was chosen from McMaster Carr. The closest diameter of lead screw that fit the diameter that was solved for was 5.97 mm, so a 3/8-10 steel acme lead screw was selected. For this assignment our lead screw is required to be at least 18 inches. The lead screw sizing selected only had 3 feet, 6 feet or 12 inches. So to accommodate for this we selected the 3 foot long lead screw and would cut it down closer to size. The lead screw we selected is linked below.
 https://www.mcmaster.com/93410A608/
### Crosshead Design and CAD - Rebekah Smith
* The objective of this portion of the project was to design a crosshead for a mechanically driven
tensile testing machine capable of applying a maximum tensile load of 2 kN. The crosshead
connects the two vertical leadscrews through bronze nut and flange assemblies and provides a
mounting location for the tensile specimen. The design required selecting an appropriate
material and cross-sectional dimensions while maintaining a factor of safety of 4 and limiting the
maximum crosshead deflection to 0.1 mm. Beam strength and deflection analyses were
performed to determine whether the proposed crosshead dimensions would meet the design
requirements.
### Crosshead Design – Beam Strength Analysis
* The crosshead was modeled as a simply supported beam with a concentrated load applied at
its center. The two bronze nut and flange assemblies act as the supports for the crosshead. The
two support reactions represent the forces from the left and right bronze nut and flange
assemblies. Because the loading is symmetrical, both support reactions are equal.
<img width="624" height="876" alt="image" src="https://github.com/user-attachments/assets/17f5eb9c-1eee-4f7f-a3e6-784a77955162" />
<img width="736" height="652" alt="image" src="https://github.com/user-attachments/assets/d0f0906a-95df-4c52-ba5c-14d30d6f3855" />

* Using static equilibrium, the support reactions can be determined by summing the vertical forces. Sum of
forces in the vertical direction: ΣFy = 0, RA + RB - F = 0 Due to symmetrical loading: RA = RB
Therefore: RA = RB = F/2 The maximum bending moment for a simply supported beam with a centered
point load is: Mmax = FL/4 The bending stress equation is: σmax = Mmax/S The allowable stress using a
safety factor of 4 is: σallow = Sy/n Rearranging the bending stress equation to determine the minimum
required section modulus: Smin = nMmax/Sy For a rectangular cross-section, the section modulus is: S =
bh²/6.
* First, calculate the support reactions: RA = RB = 2000/2, RA = RB = 1,000 N Calculate the maximum
bending moment: Mmax = (2000)(304.8)/4 Mmax = 152,400 N·mm Calculate the allowable bending
stress: σallow = 248.2/4 σallow = 62.05 MPa Calculate the minimum required section modulus: Smin =
(4)(152400)/248.2 Smin = 2,456.1 mm³ A rectangular cross-section measuring 50 mm wide and 40 mm
high was selected. Calculate the section modulus: S = (50)(40²)/6 S = 13,333.3 mm³ Calculate the
maximum bending stress: σmax = 152400/13333.3 σmax = 11.43 MPa Calculate the actual factor of
safety: FOS = 248.2/11.43 FOS = 21.71 The calculated factor of safety of 21.71 exceeds the required
factor of safety of 4. Therefore, the selected A36 steel cross-section satisfies the preliminary beam
strength requirement.
#### Crosshead Design – Beam Deflection Analysis
* The deflection analysis was performed to determine whether the selected crosshead
dimensions could maintain a maximum deflection of 0.1 mm under the applied 2 kN tensile load.
The same simply supported beam configuration and centered load were used for the deflection
analysis. The maximum deflection occurs at the center of the beam, where the tensile load is
applied. 
<img width="1006" height="886" alt="image" src="https://github.com/user-attachments/assets/9389bb90-6478-4d0c-82a7-cc2de17344da" />

* For a simply supported beam with a concentrated load at the center, the maximum deflection is:
δmax = FL³/(48EI) The area moment of inertia for a rectangular cross-section is: I =
bh³/12Substituting the moment of inertia equation into the deflection equation: δmax =
FL³/[48E(bh³/12)] Simplifying: δmax = FL³/(4Ebh³) First, calculate the area moment of inertia: I
= (50)(40³)/12 I = 266,666.7 mm⁴ Calculate the maximum deflection: δmax =
[(2000)(304.8³)]/[(48)(200000)(266666.7)] δmax = 0.0221 mm Compare the calculated
deflection to the maximum allowable deflection: 0.0221 mm < 0.1 mm The calculated maximum
deflection of 0.0221 mm is below the allowable deflection of 0.1 mm. Therefore, the selected
crosshead dimensions satisfy the preliminary stiffness requirement.
#### Crosshead Material and Dimension Selection
* A36 structural steel was selected for the crosshead because of its strength, stiffness, availability,
and ease of manufacturing. A rectangular cross-section was selected with a width of 50 mm and
a height of 40 mm. The strength analysis resulted in a maximum bending stress of 11.43 MPa
and an actual factor of safety of 21.71, exceeding the required factor of safety of 4. The
deflection analysis resulted in a maximum deflection of 0.0221 mm, which is below the
allowable deflection of 0.1 mm. Based on these calculations, the selected 50 mm × 40 mm A36
steel cross-section satisfies the preliminary beam strength and deflection requirements.
<img width="612" height="586" alt="image" src="https://github.com/user-attachments/assets/c311f55e-0c33-4ce8-963d-1a312895e0f7" />
<img width="636" height="534" alt="image" src="https://github.com/user-attachments/assets/82b35e70-fdf5-43cf-acdd-c8b4fa5a2717" />
<img width="846" height="404" alt="image" src="https://github.com/user-attachments/assets/b6ea0c67-3685-4bd7-824f-c0c53af2f58d" /> 

* A multiview engineering sketch was created to communicate the overall geometry, dimensions,
and mounting features of the tensile tester crosshead. The drawing includes top, front, and side
views to show the crosshead dimensions and the locations of the two leadscrew mounting
points. The crosshead was designed using A36 structural steel. The overall length is 12 inches,
with 10 inches between the centers of the two leadscrew mounting holes. Each mounting
location includes a 0.375-inch center hole and a 0.688-inch counterbore to accommodate the
nut and flange assembly. The counterbore depth is 0.625 inches. The crosshead has a width of
1.968 inches and a height of 1.574 inches. These dimensions provide the required space for the
mounting features while maintaining the rectangular cross-section used in the beam strength
and deflection analyses.
<img width="1226" height="732" alt="image" src="https://github.com/user-attachments/assets/4a24e3fc-f651-49af-a04a-8eb59ea473d9" />

* During the crosshead design process, I learned how to apply beam bending stress and
deflection equations to determine the dimensions required for a mechanical structure. I learned
that material selection requires considering both yield strength and elastic modulus because
strength and stiffness affect different parts of the design. One important design consideration
was selecting a crosshead cross-section that could withstand the applied tensile load while
maintaining minimal deflection. By comparing the calculated bending stress to the material yield
strength, I was able to determine the factor of safety. I also learned how the area moment of
inertia affects beam deflection and why increasing the beam height can significantly improve
stiffness. The final preliminary design uses A36 steel with a rectangular cross-section measuring
50 mm × 40 mm. The calculations showed that the design satisfies the required strength and
deflection limits. I spent around 3 hours on my portion of the assignment.
## Decide
<img width="956" height="1108" alt="image" src="https://github.com/user-attachments/assets/2f3364d3-4e1c-49e3-a103-73588480ae38" />
<img width="1014" height="1096" alt="image" src="https://github.com/user-attachments/assets/ae5758e1-c7d2-4f11-b2e5-22d34573c9a8" />
<img width="896" height="938" alt="image" src="https://github.com/user-attachments/assets/2e0ea95f-58c5-4c8b-a1c9-3381ca5bd327" />
<img width="1070" height="1100" alt="image" src="https://github.com/user-attachments/assets/191b0500-d6db-4bf9-8fba-0bac3a866838" /> 

### Nut and Flange- AC
<img width="1024" height="912" alt="image" src="https://github.com/user-attachments/assets/d79811b9-dad5-4a10-a58f-0511c997b9b6" />
<img width="1192" height="690" alt="image" src="https://github.com/user-attachments/assets/b38a947c-66c3-4770-87be-a1ef01384469" />
<img width="1262" height="930" alt="image" src="https://github.com/user-attachments/assets/053dbd2a-ff70-4605-8ba8-0a892d9020c7" />
<img width="1250" height="938" alt="image" src="https://github.com/user-attachments/assets/0aa7668c-0fd6-4cf7-a88b-22008ba2ceed" /> 

### CAD File Link 
* (CAD File Link)[A10_Tensile_Machine.zip] 

### Cost- Farima Pournia 
| Item Number | Quantity | Name | Cost/Item | Cost | Purchase Link | 
|----------|-------|-------|------|-------|--------|
| 1 | 2 | Alloy Steel Acme Lead Screw | $75.50 | $151 | https://www.mcmaster.com/93410A608/ | 
| 2 | 2 | Precision Acme Externally Threaded Nut | $29.91 | $59.82 | https://www.mcmaster.com/95072A127/ |
| 3 | 2 | Precision Acme Flange | $37.06 | $74.12 | https://www.mcmaster.com/95082A641/ | 

## Communicate
### Lessons Learned 
* Throughout this project I learned how to solve for a diameter of a part using the stress equation. I also learned how to calculate torque on a lead screw. I learned that when designing a lead screw the pitch is important throughout the calculations. I learned how to calculate the rotational speed of an object by using linear speed. I also learned how to navigate McMaster Carr well in order to select the exact component needed for the design. 
