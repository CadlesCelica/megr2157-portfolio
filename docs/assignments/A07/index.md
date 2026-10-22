# A7 – [FEA on Bracket]
## The Setup

After constructing the bracket in assignment 5, now it has to be tested.
To simplify analysis, the interior faces that contact the beam were set as fixed, and the force applied was set as acting purely in the down direction around element A.
![fixtures](<FEA  1 1 fixtures.png>)
![force and direction](<force 2.png>)
The force is listed at 1600lbs, as from the provided documentation, the strap has a tension F acting on both sides of the beam, so the total force for a tension of 800lbf is 1600 lbf.

The fixtures remain unchanged through iteration 2, so that image will be omitted.

## Initial FEA
The initial mesh density was left as the solidworks default, which is about halfway between the coarse and fine settings. 
![mesh box](<mesh 1.png>)
![mesh img](<mesh 1 img.png>)

After meshing, the FEA simulation was run.

### Run 1
![Stress 1 1](<stress 1 1.png>)

The maximum stress is 359,800 psi

![disp 1 1](<displacement 1 1.png>)
(Image should be in inches, but I did not grab the correct screenshot before continuing on)
The maximum displacement is 0.364 in

![FOS 1 1](<fos 1 1.png>)

The minimum factor of safety is 0.33

### Run 2

For the second simulation, the mesh was adjusted to medium fine.
![mesh 1 2](<mesh 1 2.png>)
![mesh 1 2 img](<mesh 1 2 img.png>)

![Stress 1 2](<stress 1 2.png>)

The maximum stress is 378,000 psi
![Disp 1 2](<displacement 1 2.png>)

The maximum displacement is 0.3663 in
![FOS 1 2](<fos 1 2.png>)

The minimum factor of safety is 0.32.

Comparing the 2 runs, the results converge within 7%.
The difference was 5% for stress, 0.6% for deflection, and 3% for the Factor of safety results.
The mass is 0.34 lbs

As can be seen, this part in its current state failed completely under FEA. This is likely due to treating component B as an axially loaded bar and failing to account for the bending induced by the applied load.

### Modifications for FEA 2

The first modification was to increase the thickness of feature B. Since the part had a FOS of 0.32, the depth of the feature was increased by 6x in order to avoid part failure.

![changes 1 1](<changed pt 1.png>)

Since many of the other features rely on feature B for geometry, they had to be modified to a new length.

![changes 1 2](<change pt 1 2.png>)

![Change 1 3](<chane pt 1 3.png>)

Feature A was also extended to fit the contours of the modified feature B.

The final modified part
![Part mod 2](<bracket 2 mod real.png>)

## FEA loop 2

The same fixed constraints apply as the first loop, and the applied force remains unchanged.

### Run 1

The initial meshing, like the first loop, started at medium density.

![Mesh 2 1](<mesh 2 1.png>)

The simulation was run, and the initial results were more promising than the first attempt. 

![stress 2 1](<stress 2 1.png>)

The max stress is 26420 psi
![disp 2 1](<displacement 2 1.png>)

The max displacement is 0.00565 in
![fos 2 1](<fos 2 1.png>)

The minimum factor of safety is 4.54

### Run 2

The mesh density was changed to medium fine, and the simulation was re run.

![mesh 2 2](<mesh 2 2.png>)

![stress 2 2](<stress 2 2.png>)

The maximum stress is 

![disp 2 2](<displacement 2 2.png>)

The maximum displacement is 

![fos 2 2](<fos 2 2.png>)

The minimum factor of safety is 

While the results are similar, they did not converge within 7%. The stress was within 16.2%, deflection 3.7%, and factor of safety 13.3%.
Since these differences exceeded 7%, the simulation was run again on the highest density mesh

### Run 3
![mesh 2 3](<mesh 2 3.png>)

![mesh img 2 3](<mesh 2 3 img.png>)

![stress 2 3](<stress 2 3.png>)

The maximum stress is

![disp 2 3](<displacement 2 3.png>)

The maximum displacement is 

![fos 2 3](<fos 2 3.png>)

The minumum factor of safety is 

Between runs 2 and 3, the results did converge. The stress was within 2.7%, displacement 1.9%, and factor of safety 2.6%.

With this knowledge, some material can now be removed without causing the part to fail. 


Loop 2, modification part 1
inner loop 1 and 2
stress 16.2%, deflection 3.7%, FOS 13.3%
On the third loop, the results of 2 and 3 converged within 7%,
Stress 2.7%, displacement 1.9%, safety factor 2.6 %

Loop 3 modifications 2
Between inner loop 1 and 2
stress 18%, deflection 0.5%, safety factor 15%
between 2 and 3
Final results did not converge, stress differed by 16.5%, deflection by 0.48%, and safety factor by 14.2%


## Analyze


## Decide


## Communicate

