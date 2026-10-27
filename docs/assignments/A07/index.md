# A7 – [Topic]

## Objective
In this assignment I will use FEA in Solidworks to improve my bracket design from a previous assignment. Throughout this process I will use the analysis in CAD to optimize my bracket so that it is lightweight but also meets all the design criteria. I will go through different iterations of the bracket in order to find the most appropriate  design choice for the constraints given. At the end of this assignment I will reflect on lesson key engineering lessons learned that I can use in the future.

## Analyze
Inner Loop:

### Fine Mesh
Max Stress 
<img width="1864" height="1116" alt="image" src="https://github.com/user-attachments/assets/b694b02a-9d97-4387-8bd3-c9034fb988d2" />
Max Deflection 
<img width="1806" height="1034" alt="image" src="https://github.com/user-attachments/assets/7616b51c-bb3d-4eae-829c-0b3dc9bdba30" />

### Medium Mesh 
Max Stress 
<img width="1834" height="978" alt="image" src="https://github.com/user-attachments/assets/a5b488d9-322d-430d-b23f-ee2ba384aa21" />
Max Deflection 
<img width="1802" height="932" alt="image" src="https://github.com/user-attachments/assets/56fc650c-2586-4a1c-bd85-97a2892b3e95" />

### Coarse Mesh 
Max Stress 
<img width="1936" height="982" alt="image" src="https://github.com/user-attachments/assets/5fe3201e-7785-414d-880d-be5f4b3fc128" />
Max Deflection 
<img width="1862" height="924" alt="image" src="https://github.com/user-attachments/assets/911cc300-b5f4-43b0-87ec-664e4338fc62" />

<img width="2500" height="1072" alt="image" src="https://github.com/user-attachments/assets/ea585dd1-942e-4b60-bb44-ed0ac9c37125" />

* The results from the the three rounds of inner loop iterations converge within %7, as a result outer loop iterations were started. 
 

## Decide
Outer Loop: 

<img width="1488" height="870" alt="image" src="https://github.com/user-attachments/assets/d1553b42-c71b-42db-ac9b-b3cc48cf5c53" />
* The finalized mesh was chosen based on the results from the inner loop and convergence test. This Mesh sizing was then used for all the design iterations of the outer loop as it followed the convergence test.

### Design 1:
Max Stress 
<img width="1956" height="924" alt="image" src="https://github.com/user-attachments/assets/9fcdb84e-1817-4c3f-8a11-df07f447809f" />
Max Deflection
<img width="1932" height="930" alt="image" src="https://github.com/user-attachments/assets/d8ca3ae4-879f-47cc-8095-6bb369ade4d7" />
Safety Factor 
<img width="1904" height="896" alt="image" src="https://github.com/user-attachments/assets/bac2bbad-a3c4-4379-a221-55ea73a039ab" />

### Design 2
* The walls on the left and right side of the bracket were made thinner in order to create a more lighter design. Throughout the simulations the walls on the side showed no issues with hitting a low safety factor or experiencing a lot of stress. As a result it was concluded that the extra thickness on the sides could be cut down. 
<img width="1420" height="916" alt="image" src="https://github.com/user-attachments/assets/a97933e8-7b85-40f3-a16f-be300b8796cc" />
Max Stress 
<img width="1862" height="904" alt="image" src="https://github.com/user-attachments/assets/4d02ec3e-d74c-43f5-b853-e2f8b515e89b" />
Max Deflection 
<img width="1872" height="848" alt="image" src="https://github.com/user-attachments/assets/d5747929-0b45-426e-8177-aa9118ba662f" />
Safety Factor  
<img width="1884" height="816" alt="image" src="https://github.com/user-attachments/assets/47c58e6b-a956-4a6e-a3a7-fade692aee0e" />
* Taking out the material lowered the weight of the car by a quarter of a  pound. Although a significant amount of material was removed it did not effect the brackets ability to carry load, the material that was taken out was done specifically in a area that would have the least effect on the structural integrity of the bracket. After this design iteration it can be concluded that much more material can be removed from the bracket without harming the over structural integrity of the bracket. 

### Design 3
* In this Design iteration the thickness of the top of the bracket was decreased in order to decrease the weight. This part of the bracket was chosen because in the simulations it does not yield under any of the forces, meaning that most likely more material can be taken out of this section. 
<img width="1530" height="970" alt="image" src="https://github.com/user-attachments/assets/b2f1201a-26b6-4218-b245-3d8bf3692fa3" />
Max Stress 
<img width="1888" height="1002" alt="image" src="https://github.com/user-attachments/assets/2f6e1980-e6e4-4ddb-b5b0-00ddd18714fd" />
Max Deflection 
<img width="1846" height="994" alt="image" src="https://github.com/user-attachments/assets/eb693bb6-c874-40d2-bce6-808703b07638" />
Safety Factor  
<img width="1782" height="898" alt="image" src="https://github.com/user-attachments/assets/402481b9-716a-40d7-b4b8-fa44a7a35ad4" />
 * This design iteration slightly increased the max stress and increased the max deformation by a noticeable amount. Even though it seemed to have had a negative effect on the numbers it still stayed within the safety factor while also cutting down the wait almost a full pound from the original starting weight. 
<img width="2516" height="1060" alt="image" src="https://github.com/user-attachments/assets/df2ce528-6212-431f-b03a-3ec0399f456b" />

## Communicate
* Through this assignment I learned how different mesh sizes can effect the accuracy of a simulation. I also learned the pros and cons to having ether a more coarse or a more fine mesh, such as simulation time versus accuracy. I also learned how to use simulation results to further guide my design process and iterations. By using the different scenes, stress, deflection, and safety factor I was able to pin point what parts of my component could be taken out in order to make my component lighter but maintain it's structural integrity. 
* I spent 5 hours on this project.

### Finalized CAD File 
[https://github.com/fpournia-png/megr2157-portfolio/blob/main/docs/A7_Bracket.SLDPRT]

