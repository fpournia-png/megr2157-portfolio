# A11 – Motor Selection

## Objective
* The objective of this project is to design and develop a functional tensile testing machine capable of applying a maximum tensile load of 2 kN to evaluate the mechanical properties of materials. The design incorporates a lead screw drive system, stepper motors, a structural frame, a movable crosshead, and appropriate mounting components to safely and effectively apply the required load. The project involves selecting and sizing mechanical components, performing engineering calculations and free-body diagrams, evaluating structural integrity through finite element analysis (FEA), and creating a complete SolidWorks assembly. Each team member is responsible for specific portions of the design while collaborating on the final assembly, bill of materials, engineering costs, and project documentation. The final goal is to produce a complete, well-documented design that meets the project requirements while demonstrating the application of mechanical engineering principles.

## Analyze
### Frame Connections, Bracket Design, and Top Frame FEA - Bekah 
#### Design Responsibilities: Structural frame connections, motor twisting analysis, mounting bracket design, and top frame structural verification.
#### Design Objective
The objective of this portion of the project is to design and analyze the structural connections between the vertical supports and the top frame of the tensile tester. The frame must support the applied tensile loads while maintaining sufficient strength and stiffness to prevent excessive bending, twisting, or deformation during operation.
The analysis focuses on the forces and moments transferred from the two motors into the frame, the structural integrity of the mounting brackets and fasteners, and the ability of the top frame to withstand the applied loading conditions. Hand calculations and free-body diagrams are used to determine the forces and moments acting on the connections. SolidWorks Simulation is then used to evaluate the top frame through finite element analysis (FEA), including von Mises stress, displacement, factor of safety, and mesh convergence.
#### Known and Unknown Variables
The following known variables were identified before beginning the frame connection and structural analysis, and the variables that must be determined through engineering calculations or SolidWorks Simulation.
<img width="760" height="826" alt="image" src="https://github.com/user-attachments/assets/b6da24a0-4e68-4b33-bbc3-dbc34733b5b4" /> 

#### Frame Connection and Motor Twisting Analysis
The tensile tester uses two identical stepper motors positioned above the lead screw system. Both motors are mounted with their shafts oriented vertically downward. The center-to-center spacing between the motor and vertical support locations is 9.62 inches.
Each motor drives a lead screw that contributes to the movement of the crosshead. The two lead screws share the required tensile load, resulting in an axial load path of 1,000 N per lead screw under the 2,000 N maximum loading condition.
In addition to the axial loading, the motor mounting arrangement introduces reaction torques into the frame. These reaction torques must be considered because they can cause twisting or warping of the top extrusion and place additional loading on the mounting brackets.


### Vertical Frame FEA 
* For this part for the assignment I conducted FEA on the vertical components of the frame in order to analyze the effect forces will have on our frame. I used Solidworks to conduct this analysis and run my simulation. I first isolated one of the vertical columns in CAD and then assigned the correct material of 6063-T4 Aluminum then proceeded to assign two forces to the column. I applied one axial compression force of 2 kN as a result of the top of the frame pushing down on the column. The second force I added to the simulation was the torque of 6 N that the motor will exert on the column, this force was added to the side of the column around the center axis. After assigning my forces I proceeded to add in a fixed fixture for the bottom of the column.
<img width="518" height="1098" alt="image" src="https://github.com/user-attachments/assets/ea6de894-9b1c-49b1-afd9-22bc7eacac14" />

* In order to run a convergence check I ran two simulations with two different types of mesh. My first simulations started out with a mesh sizing directly in between fine and coarse mesh size. After running the sim gathered data about the stress scene that showed the variation of stress across the whole column. This scene showed that the max stress was located at the bottom corner of the column at around a value of 6x10^6 N/m^2. The next scene I look at was deflection across the column at around 0.14 mm. The max deflection was at the top corner where the compressive force is being applied also at the same corner where the max stress was. The next scene that was created was a safety factor scene that allowed me to see how close our design material and vertical column was close to the limit of the safety factor for this design. The entire column was well within the safety factor. 

<img width="372" height="1060" alt="image" src="https://github.com/user-attachments/assets/b1a702c7-8b34-4d6e-8d91-1625a7703edb" /> 
<img width="1246" height="1070" alt="image" src="https://github.com/user-attachments/assets/a3b0ec26-108e-4f2c-ac9f-5dd601d849ec" /> 
<img width="1138" height="1068" alt="image" src="https://github.com/user-attachments/assets/92d90a13-1d44-4999-8588-0c72139af1c5" /> 
<img width="1086" height="1016" alt="image" src="https://github.com/user-attachments/assets/4212b703-6e50-41df-a369-35f7f36f07bf" /> 

* For my second simulation I ran a more fine type of mesh in order to complete my convergence check. This time I made the mesh size halfway between the middle and fine mesh size, this should give us more accurate results in the simulation. After the simulation I analyzed different scenes that were shown. The first one I analyzed was the stress scene which showed a max stress of 6.25x10^6 at the bottom corner which is at the same location of the previous sim. The second scene I looked at was deflection in the column. The max deflection is 0.14 mm at the top corner of the column at the same point above where the max stress is, this looks very similar to the other simulation that was ran but with a higher area of max deflection. The safety factor of the column is met in all locations which is confirmed by the safety factor scene shown, which also matches with the other simulation. 

<img width="444" height="1024" alt="image" src="https://github.com/user-attachments/assets/3af5ebab-b812-4801-994e-b82e463171c1" />
<img width="1254" height="1052" alt="image" src="https://github.com/user-attachments/assets/c5af6949-36df-4559-8585-a3544f422775" /> 
<img width="1178" height="1050" alt="image" src="https://github.com/user-attachments/assets/10d6dd93-6b5e-4e3f-8531-6ed9dfd7cadc" /> 
<img width="1070" height="1034" alt="image" src="https://github.com/user-attachments/assets/7536c656-c5c9-4105-a1b7-c99234dd0d08" />


* Overall the simulations between the two different types of meshes matched up results very well. The locations of the max forces and deformation lined up and the numbers of the maximum forces and deflection were within 5 percent of each other. The safety factors also looked exactly the same between the two meshes. One main difference that I noticed between a fine or coarse mesh was that a more fine mesh always calculated a higher deflection or stress and usually in a slightly larger area. The increase in cells allow the sim to be more accurate and to account for forces that may have been missed with a more coarse mesh. After running these simulations I noticed a couple of trends throughout the different scenes. One was that the location of the max stresses and deflections were always in the corner. Another was that the beam had a tendency to twist around it's axis starting from the top where the torque is first applied and decreasing till the bottom. Some changed to add in order to make the column more structural sound could be adding thicker flange pads at the top where the column experiences the most amount of torque. The most amount of deflection and stress was seen at the top of the column where the torque from the motor was experienced. 

### Floating Bearing Mount 
* To design the floating bearing mount, I made the thickness 0.25 inches. The length is 3 inches with a width of 2 inches that will fit on the aluminum bar. The mount has a hole in the middle for the lead screw is set to 0.3 inches with a tolerance of +- 0.0005 from the Machinery Handbook. There are 4 holes on the mount for #10 screw, the diameter of the screws is 0.2 inches. 
<img width="1060" height="1054" alt="image" src="https://github.com/user-attachments/assets/1f13231e-337a-4ad6-a4e0-c524cbc64ecb" />
<img width="848" height="1138" alt="image" src="https://github.com/user-attachments/assets/bf05c468-df9b-4171-a4c8-aa9c95532fa2" />

## Communicate
* I spent 5 hours on this assignment. 
