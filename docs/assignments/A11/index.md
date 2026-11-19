
# A11 – Motor Selection

## Objective


## Analyze
[bracket download](<A11 Motor Bracket1.SLDPRT>)


## Decide
_Reference your concept selection (Pugh matrix) here. How does this design follow from that decision?_

## Communicate

## Frame FEA - Aidan Cadle

The top of the frame was analyzed to ensure adequate strength and minimal deflection given the 2kN axial load and moments induced by the 2 chosen electric motors.
The stall torque from the electric motors data sheet was used in order to design for the 'worst case' scenario.
In an attempt to accurately conduct the FEA, the column brackets were mated to a double 40 series beam, as that is how our frame is assembled.

<img width="1208" height="675" alt="assembly" src="https://github.com/user-attachments/assets/8823af9d-7c54-43ae-8eb3-ab57159320ff" />

The column brackets were set as fixed geometry, and center holes were placed where the leadscrews would go. 

<img width="1126" height="679" alt="load" src="https://github.com/user-attachments/assets/1d330bed-9bd8-4517-8daa-32d4957ec5e3" />

Then, the FEA was attempted. However, unlike previous assignments, the end results were not clear. The first pass was conducted on the coarse setting within Solidworks.

### Initial Results
<img width="1896" height="895" alt="assembly fea test" src="https://github.com/user-attachments/assets/9dc6ef62-87aa-4227-89dc-e4892c214e15" />

Stress

<img width="1851" height="748" alt="assemb disp" src="https://github.com/user-attachments/assets/5274ca81-42d9-4df6-8551-52769f7926d4" />

Strain

<img width="1749" height="725" alt="assemb FOS" src="https://github.com/user-attachments/assets/0314cbf7-c434-475e-bd64-e593155fd56b" />

Factor of Safety

As can be seen in both the stress and factor of safety images, there is almost no color variation, and yet the plot ranges all the way to 21 GPa, well outside of the yield strength of aluminum.
Despite this, the deformation plot seemed to be accurate, showing gradual variation, and a peak displacement of only 0.0078 mm. 

In an attempt to fix this, a finer mesh was used. However, despite multiple attempts, Solidworks would not run the same simulation on a finer mesh

<img width="253" height="159" alt="fea failure" src="https://github.com/user-attachments/assets/522d5d37-0f36-4aba-970c-5d5309bbb27d" />

One of many error codes.

### Second Assembly Configuration

Since motor mount plates were designed and now available as Solidworks parts, those were added to the assembly in an attempt to resolve this issue.
The loads were applied through the motor mounts, as that is how the loads would be distributed on a physical frame.

<img width="1126" height="679" alt="load" src="https://github.com/user-attachments/assets/a32800f1-f8ca-478d-bfb5-f5152bfeac0f" />

Despite the computer's best efforts, often exceeding 77 degrees Celsius, this did not solve the problem. The stress and factor of safety again came out monochromatic, and the displacement plot appeared to be properly scaled. 

<img width="1399" height="1026" alt="run 2 stress" src="https://github.com/user-attachments/assets/c3a09a4f-b1e2-4c34-99e3-aa0f6f98469f" />

Stress

<img width="974" height="854" alt="disp 2" src="https://github.com/user-attachments/assets/b105fcad-b126-4873-b796-ec24b47e27e6" />

Displacement

<img width="923" height="787" alt="run 2 fos" src="https://github.com/user-attachments/assets/ef921a3f-ead0-45fc-8688-d00563f25cca" />

Factor of Safety

In addition to adding the motor mounts, the scale of the charts were adjusted in an attempt to view a rough idea of the maximum stress. The upper limit was set to that of the yield strength of aluminum, 275 MPa. Despite this, the charts remained monochromatic. 

A finer mesh was used, however the computer took over 10 minutes to complete it, and the results were not significantly different or more conclusive than the coarser mesh. 

### Final Assembly Config

In a final attempt to 'correctly' conduct the FEA, the column L brackets were removed, but the motor mounts remained. In this configuration, the ends of the beams were treated as fixed geometry, but the loads were still applied through the motor mounts. 

<img width="1494" height="639" alt="fea 3 fixtures" src="https://github.com/user-attachments/assets/970bdc74-9c3b-4730-b666-b2002dd5109e" />

The model was meshed on coarse, and the FEA simulation was run.

Worth noting, for every FEA conducted for this assignment, Solidworks always had a warning pop-up saying the mesh contained distorted elements. It did not matter the mesh density, although the number was generally higher the finer the mesh.

Despite the new constraints, the results did not change.

<img width="954" height="815" alt="stress 3" src="https://github.com/user-attachments/assets/7682a2e5-3b67-4408-9a6b-fef135e2951f" />

Stress

<img width="961" height="684" alt="disp 3" src="https://github.com/user-attachments/assets/a3b7a37a-64ce-4d45-a129-12345c29964e" />

Displacement

<img width="946" height="747" alt="fos 3" src="https://github.com/user-attachments/assets/6dc3dd94-c7df-400d-b377-eabed9693d21" />

Factor of Safety

The stress plots appear to be inconclusive, but the displacement plots tell another story. They show minimal deflection in every test, suggesting that the beam is indeed rigid enough to support the given loading. 

### Final FEA attempt

In a final attempt to gain usable data, FEA was conducted on the beam only. 
The ends were set as fixed geometry, and the force and torque were applied around vertical walls of the clearance holes for the lead screw. 

<img width="1690" height="748" alt="part load and fixture" src="https://github.com/user-attachments/assets/eea4604a-a9a6-4575-9abb-d870cb1e797c" />

The mesh was set to coarse, and the simulation was run.

Finally, the simulation resulted in usable results. 

<img width="1343" height="604" alt="stress" src="https://github.com/user-attachments/assets/4cbf3bea-dc82-489a-87c7-e621e50480d8" />

Stress. Peak 116 MPa

<img width="921" height="785" alt="disp 4 1" src="https://github.com/user-attachments/assets/5d3477e2-33c1-4c7e-b224-1d8f16f87094" />

Displacement. Peak 0.042 mm

<img width="860" height="744" alt="fos 4 1" src="https://github.com/user-attachments/assets/7bfd108c-3cc7-4b0e-88b1-1f793c86c582" />

Factor of Safety. Minimum 2.4

All plots now show a gradient, and appear to show correct stresses and factors of safety. Now, the mesh was refined in order to gather more data, and to look for possible convergence. 

According to Solidworks, for both the coarse and medium fine mesh, there were no distorted elements. This is significantly different than the previous attempts.

<img width="1408" height="772" alt="stress 4 2" src="https://github.com/user-attachments/assets/624aaf54-e8e6-459a-bc28-549fecbecbe2" />

Stress. Peak 120 MPa

<img width="885" height="749" alt="displacement 4 2" src="https://github.com/user-attachments/assets/f9c8475b-8f38-46aa-b097-b790300c0b3e" />

Displacement. Peak 0.042mm

<img width="845" height="690" alt="fos 4 2" src="https://github.com/user-attachments/assets/dd7f1997-425c-49da-af73-44d4b0366bf7" />

Factor of Safety. Minimum 2.3

These values converge within 4.2% of one another, so further refinements are not necessary. 






