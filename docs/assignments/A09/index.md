# A9 – Pulleys

## Objective
In this assignment the goal was to design a pulley system that transfers power between two parallel axes separated by a chosen distance of 5 inches and a chosen material of aluminum for the pulleys and polyurethane rubber for the belt. The pulley had to be designed to meet a set of parameters like the pulley diameter, rotational speed, belt tension, and safety factor. Fundamental equations for solid mechanics and the parameters given were used to calculate the information needed to design the pulley system. The frame, belt, and shaft were all designed while the calculations for the journal bearing were used to select the correct journal bearing from McMaster Carr. 

## Analyze

### Belt 
* The first part of the assignment was to design and select a belt from McMaster Carr that met the parameters given. The material of the belt was polyurethane rubber and which was used to find the coefficient of friction from the Machinery Handbook. To select the correct belt needed for the pulley system the forces on each pulley, the diameter, area, and circumference of the belt needed to be calculated. Two main equations were used for these calculations, these equations were both solved for one variable and set equal to each other. Solving for one forced allowed me to solve for the second force and then use the stress equation to solve for area of the belt and in turn the diameter. I then used the diameter to find the circumference of the belt.
<img width="2180" height="1772" alt="image" src="https://github.com/user-attachments/assets/78d68fb6-8ad9-453c-9440-6d770818966b" />
<img width="1940" height="904" alt="image" src="https://github.com/user-attachments/assets/699c0dfc-4ca4-46d7-854a-4f57e0e37b80" />

* After all these variables were calculated I then proceeded to input these parameters in McMaster Carr to find the best fitting belt for the pulley system. The correct belt was selected by selected rubber as the material and selected the belt that has the closest diameter and circumference to the one calculated. The diameter calculated was 0.279 inches and the belt with the closest diameter was 5/16 inches. The circumference calculated was 20.30 inches and the closest circumference was 20.50 inches. The image below is the belt that was selected.    
<img width="1770" height="916" alt="image" src="https://github.com/user-attachments/assets/0089de9b-64fa-4427-8b98-b7a38a9179a2" />

### Shaft 
* The second component of the pulley system that was designed was the shaft. The materials of the shaft is 1060 hardened steel which allows us to know the shafts yield strength. The power equation was used to solve for torque, and these variables were then plugged into the shear stress equation. The area variable of the shear stress equation was converted to the equation for area of a circle and the diameter was solved for.
<img width="2080" height="1860" alt="image" src="https://github.com/user-attachments/assets/56b36eeb-b393-4546-9735-cb2823e28775" />

## Decide

### Journal Bearing 
* I went through a series of calculations in order to select the correct journal bearing from McMaster Carr for the pulley system. I solved for the PV rating, pressure and linear velocity in order to use these variables to decide on the correct type of journal bearing to be selected. Pressure was first calculated by dividing F1 and F2 by the area. To find the PV rating I needed linear velocity so I converted the rpm I chose of 1500 to angular velocity and then converted angular velocity to linear velocity.
<img width="2104" height="1464" alt="image" src="https://github.com/user-attachments/assets/0b0353c1-c25d-4feb-bea1-3ee672489128" />

* Using the PV rating and the table of journal bearings in the Machinery Handbook I was able to select the correct type of material for my journal bearing. I selected graphite for my material because the PV rating of graphite is much higher than what was calculated meaning that the material should have no issue handling the forces it will experience.
  
### Frame 
* I used the design given in the resources of the assignment as a baseline for my frame. I selected Aluminum as my material because it is easy to machine and fairly light weight. To establish the correct dimensions for the frame I selected preliminary dimensions and went through calculations to ensure what I had selected would handle the forces the frame would experience. I solved for stress and then made sure that the stress solved for was within the safety factor. I then solved for deformation using the area I calculated and the combined forces that the frame would experience. My last calculation consisted of taking into account the holes where the shafts were located. I did this by subtracting that area from the full length of the frame and solving for stress and confirming that it is still within the safety factor. 
<img width="2392" height="1516" alt="image" src="https://github.com/user-attachments/assets/4dc409a8-8fd8-4ac7-aee9-5f8a7c756e61" />

## Communicate

### Lessons Learned 
* Throughout this assignment I learned about how a pulley system is designed and important parameters to consider. I learned through belt selection what parameters were needed to select the correct type of belt. I also learned how to relate force and friction equations to each in order to solve for forces, and I learned how I have to take into account the combined force of both the loose and tight end of the belt when doing my calculations. For the shaft design I learned how power and angular velocity relate to torque. For the journal bearing I learned the difference between angular and linear velocity and how to go from rpm to linear velocity. In frame design I learned that I have to take into account gaps in my part when calculating stress because stress is heavily dependent on area. 
* I spent 8 hours on this assignment. 

