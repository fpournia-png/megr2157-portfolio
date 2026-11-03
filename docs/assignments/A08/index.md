# A8 – Gears

## Objective
The objective of this assignment is to design and create a gear box that can be assembled and disassembled easily. Use the parameters given to analyze and size the input and output shaft and to design a journal bearing that meets the specification necessary. Finally, this design must be modeled in CAD.

## Analyze

I used the Machinery Handbook to look up the values of maximum shear yield strength for a power transmitting shaft and a short staff. I used the diameters given for output and input shaft, and the gear ratio to calculate the amount of torsion that these shafts would experience. I then compared the torsion values I calculated to the maximum shear yield strength values each type of shaft was rated for. If the values I calculated were below the maximum shear yield strength the shaft is rated for then the diameter is sufficient, but if they are above then the diameter must be changed as the shaft exceeds the load it's rated to receive.  
### Input Shaft 
<img width="2004" height="1556" alt="image" src="https://github.com/user-attachments/assets/37fbb07f-0875-41a3-ad73-6a4c1f9cde78" />

* The amount of torsion that a 0.125 inch diameter input shaft will receive under the conditions of this problem is less than the amount of maximum shear yield strength it is rated for. As a Result, the 0.125 inch diameter is sufficient for this application and the diameter size does not need to be changed. 

### Output Shaft 
<img width="2224" height="1292" alt="image" src="https://github.com/user-attachments/assets/370cde69-e7b4-42df-a3f5-732ccf2d5d40" />

* The amount of torsion that a 0.25 inch diameter output shaft will receive under the conditions of this problem is less than the amount of maximum shear yield strength it is rated for. As a Result, the 0.25 inch diameter is sufficient for this application and the diameter size does not need to be changed. 

## Decide

### Journal Bearing 
A journal bearing is a type of bearing that supports a shaft and allows it to rotate with minimal friction, allowing for more efficient power transfer. The following are the equations, and data that I used to make a decision about the appropriate size, length, and thickness of the journal bearing under the conditions of this problem. These calculations allowed me to chose a journal bearing that would correctly work in the application of this assignment. 
#### Size and Length 
* For my journal bearing length I chose 0.20 inches. I went through several calculations to come to a conclusion of what material should be used for the input and output shafts. First, I used the information given to calculate what the highest force acting on the bearing would be. Then I calculated the maximum pressure by using the highest force that the bearing would experience and dividing it by the area that was calculated from the diameter of the shaft and the length that I chose. Finally, I calculated the velocity and PV value using their respective equations. To decide on what materials to use for the input and output shafts I looked in the table in the Machinery Handbook. I looked at the pressure, velocity and PV values listed under each material in the table and then proceeded to chose my material by making sure the values I calculated were well below what the material could handle.
<img width="2280" height="2220" alt="image" src="https://github.com/user-attachments/assets/3dc5433a-fe12-4e38-a819-fc205ab447ff" />

* The material I chose for the input shaft is porous bronze and dry graphite for the output shaft. These materials were chosen because the pressure, velocity and PV values in the table are well above what the bearings will experience which means it is an appropriate material to chose as it would handle the forces.
  
#### Thickness 
To calculate the minimum thickness necessary for the bearing I used the stress equation. For area I used the length I chose as one variable and represented the thickness with the variable t. For the stress value I used the table in the Machinery Handbook and found the maximum stress values of the materials that I chose in the section above. I then used the radial force that I had previously calculated to isolate the t variable for thickness and solve for the thickness necessary to support the forces that the bearing will experience. 

<img width="2192" height="2292" alt="image" src="https://github.com/user-attachments/assets/ca27bac9-7bd7-46d4-9a01-b8134f030695" />
<img width="2536" height="792" alt="image" src="https://github.com/user-attachments/assets/870d54ff-9195-46d8-af31-611a84d636d4" />

* The McMaster Carr journal bearing component for the input shaft is, and 2867T41 for the input shaft. 
<img width="1472" height="1876" alt="image" src="https://github.com/user-attachments/assets/a58da7e7-a41b-43da-a5e3-a5da36d36e44" />

* CAD Model:(A8_GearAssembly(1).zip) 
<img width="1346" height="898" alt="image" src="https://github.com/user-attachments/assets/190d156e-18af-4fdf-8f33-4912e5f98baa" />
<img width="1310" height="1014" alt="image" src="https://github.com/user-attachments/assets/a3410c1f-f3ec-4b93-ab33-cc4f53071f7d" />
<img width="996" height="960" alt="image" src="https://github.com/user-attachments/assets/57d866fc-da4e-41ec-b7fa-0b7848471c86" />

## Communicate
### Lessons Learned 
* Through this assignment I learned many lessons about what goes into designing a gearbox. I learned about what forces the gears experience as they spin against each other. I learned how to use the gear ratio to obtain other information about gears. I learned the importance of a journal bearing and the importance of the material that is chosen for it, and what factors go into that decision. I learned how to use McMaster Carr to select the bearing that I needed. Finally I learned what a gear box is, how the two halves of the gear box can be assembled, and how I can model it in CAD. 
* I spent 8 hours on this assignment. 
