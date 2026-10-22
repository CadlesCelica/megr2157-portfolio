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
The maximum stress is 
![Disp 1 2](<displacement 1 2.png>)
The maximum displacement is 
![FOS 1 2](<fos 1 2.png>)
The minimum factor of safety is 0.32.


Converged after 2 simulations
Stress within 5%, deflection 0.6%, FOS within 3%


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

