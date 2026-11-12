# A10 – Lead Screw Tensile Tester

## Crosshead Design - Aidan Cadle

In building the tensile tester, the crosshead had to be designed with a factor of safety of 4, a maximum deflection of 0.1 mm, and support a tensile load of 2 kN. Given the constraints and example of "low cost" testers, the chosen material is 6061-O Aluminum, and the center to center distance between the two lead screw holes is 8 in. 
6061-O Aluminum has a yield strength of 62.05 MPa, and an elastic modulus E = 69 GPa.

![calc 1](<A10 Scans_page-0001.jpg>)

Initially, the calculations assumed a square cross sectional area. However, this would lead the flange to "stick out" from the crosshead and mount incorrectly, so the calculations were repeated using a rectangular cross sectional area. 

![calc 2](<A10 Scans_page-0002.jpg>)

Calculations were repeated, but now the width of the crosshead was set to 1.6 in, the outer diameter of the flange. Using the equations for a fixed beam with a load in the center, calculating for both stress and strain, the minimum height of the crosshead was determined to be 0.866 in. 

Under the calculations, the rough multi angle sketch, with a top, front, and right view is included. While not specifically labeled, the material of the crosshead is 6061-O Aluminum, as described above. 
Holes are included for the lead screws, flange mounting, and specimen mounting solution. 

## Parametric Modelling

### Crosshead - Aidan Cadle

For the 3D model, the part was parametrically calculated.
Variables and equations were defined for every useful value needed within the calculations.

![eqn](eqn.png)

After all of the variables, equations, and metric to imperial conversions were applied, the result matched that of the previously calculated value.

Now, the sketch can be defined using these variables and calculated values.

![sketch](<bar sketch.png>)

The sketch was then extruded out using parametric techniques.

![ext](extrude.png)

The final part, parametrically produced. 

![Part](<part iso.png>)


