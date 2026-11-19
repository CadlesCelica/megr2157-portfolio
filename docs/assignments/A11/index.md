
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





