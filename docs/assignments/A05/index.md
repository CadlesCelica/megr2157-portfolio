# A5 – [Bracket Analysis and Design]

## Stress analysis of Bracket

To simplify analysis, a few assumptions were made. The material selected is titanium, the applied force is 800 lbf, no failure from shear stress, the maximum deflection in any feature has to be less than 0.005 in, the factor of safety is 4, and the mechanics of each feature were simplified for design. However, all analysis was conducted with a safety factor of 5, as I did not initially find the factor of safety in the listed parameters. 

### Feature A

For feature A, is was treated as a cantilever bar with a distributed load. The length of the bar is assumed to be the width of the strap that it supports, which is 0.75in. This leaves the diameter of the bar as the only unknown.
E = 15,200 ksi, Sy = 120 ksi

![stress comp a](<A5 SoDesignpage0001.jpg>)

Stress, deflection, moment of inertia, and section modulus were all derived from the Machinery's Handbook. 
Using the equations and known properties of Titanium, the minimum diameter was determined to be 0.634in.

### Feature B

After determining the diameter for part A, I started on the stress analysis for part B. However, I did not finish it, and came back to it a few days later. When I came back, I could not find my train of thought, so analysis for feature B was restarted. Again, to simplify analysis, the width of feature B was set to the diameter calculated in feature A, and the overall height was set to 2x the diameter, or 1.268in.

![comp b and c](<A5 SoDesignpage0002.jpg>) 

Feature B was treated as an axially loaded bar, and the resulting stress analysis resulted in a thickness or depth of 0.1052 in.

### Feature C and D

Feature C was treated as a simply supported beam with a concentrated load in the center. The width was determined by the minimum measurements outlined by the T-beam, which has a total width of 2.496 in. The depth was determined by the length of feature A to simplify packaging and analysis, so the depth = 0.75in

![comp c and d](<A5 SoDesignpage0003.jpg>) 

The cross section was sketched to ensure correct orientation of the section modulus, and the final minimum height was determined to be 0.577in. 

For feature D, the bracket was split symmetrically down the center, and each side was treated as an axially loaded bar with half of the total load applied by the strap. The height was established by feature C in the t-beam, which is 1.499 in, and the length was again determined by the length of feature A on the bracket, which is 0.75 in. 
This resulted in the final width of feature D being 0.0444in on each side, increasing the total width of the bracket by 0.0888 in.



![comp e and draw](<A5 SoDesignpage0004.jpg>) 
![Strain a and B](<A5 SoDesignpage0005.jpg>) 
![comp c and d deflect](<A5 SoDesignpage0006.jpg>) 
![comp e and draw delfect](<A5 SoDesignpage0007.jpg>) 
![bracket and analysis](<A5 SoDesignpage0008.jpg>)
