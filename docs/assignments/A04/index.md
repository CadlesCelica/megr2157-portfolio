# A4 – Motor Mount and Technical Drawing

## Objective
For this assignment, the students were tasked with designing a vertical motor mount for an electric motor, constructed of 2 different elements. These two elements are a horizontal cantilever beam on which the motor rests, and a vertical beam that securely attaches the motor to the wall. The weight of the motor was not considered in the design.

![Writing Page 1](<a4 pg 1.jpg>)

While the material listed in the written document is ABS or PLA, the final chosen material is PETG, and that is the origin of the mechanical properties listed in the problem. 

[PETG Data Sheet](https://devel.lulzbot.com/filament/Rigid_Ink/PETG%20DATA%20SHEET.pdf)

## Analysis, Loading
The minimum length of the first feature is 28mm, as that is the maximum width of the electric motor. The minimum height is 2.5mm, found from subtracting the keyway length and boss length from the total length of the shaft. 
To simplify the analysis, the applied force is treated as an axial load on the first feature, so the axial stress and deflection equations are used to find the minimum width of the base.

![Paper no 2](<a4pg 2.jpg>)

The minimum width, as found from the deflection equation, is 15.4mm. This accounts for both the safety factor, and a hypothetical maximum stress concentration factor of 3. However, to avoid any overhang and to ensure proper mounting area, the minimum width was set to 28mm, equal to that of the electric motor. 

Since the second feature is solidly mounted with an overhang, the applied force is treated as an induced moment, with F = 300N and r = h = 2.5mm, for a total moment of 0.75 N m. *While editing the portfolio, an error was noticed in one of the formulas. Correcting this results in the final width of feature 2 being 4.54mm instead of the previously calculated 1.86mm*

![Paper 3](<a4 pg 3.jpg>)

Since the incorrect measurement was used in the construction of the sketch, the second feature retains the original 1.86mm width instead of the corrected width.

![iso sketch](<a4 pg 4.jpg>)

## CAD
Before the part is constructed, all appropriate equations and variables are defined. 

![Cad eqns](<a4 equations.png>)

To start, a base of 28x28mm was constructed. This was inspired by other motor mount designs, and leaves no overhang of the motor itself.

![f1 sketch](<A4 f1 sketch.png>)

This works, as the minimum required width of the beam from the calculations is 15.4mm. Additionally, one hole for the shaft is added, with a nominal diameter of 6mm. The screw holes for the motor are then added, with a nominal clearance of 3.4mm

![f1 extrusion](<A4 extrusion.png>)

The first feature is then extruded 4.5mm up from the top plane. This is so that the keyway portion of the motor shaft is exposed, and the solid shaft passes through the beam, and so that the boss of the motor sits flush with the mount. 

![boss cut](<f1 boss.png>)

For the second feature, it retains the same width as the first feature, being 28mm. The height is 94.6mm, determined from the maximum possible height of the motor from its tolerances. 

![f2 sketch](<A4 feat 2 sketch.png>)

Using beam bending and deflection equations with the given force of 300N and a calculated lever arm of 2.5mm equal to the depth of material at the boss of the motor, the minimum depth of the part is 4.54mm, verified by the equation inserted in Solidworks. This comes from the maximum stress equation, as it produced a higher value than the deflection equation.

![f2 extrude](<f2 extrude.png>)

Assuming the bracket mount holes need to be the same clearance as the motor screw holes, 4 are added with a hole diameter of 3.4mm

![f2 cuts](<f2 cuts.png>)

## Technical Drawing

![Drawing Final](<tech draw final a4.png>)

## Part and Drawing Links

The Solidworks part can be found [HERE](<A4 part Cadle.SLDPRT>) and the Drawing can be found [OVER HERE](<A4 part DRAW.SLDDRW>)

## Lessons Learned
My dimensioning on Solidworks is rusty, and needs improvement to reach an adequate level for employers. Additionally, I need to pay close attention in the transformation of equations, as a variable or integer can be easily omitted in a rush. 

Total time: 4 Hours calculations and brainstorming, 4 hours CAD and portfolio for 8 hours total on this project.






