# A5 – [Bracket Analysis and Design]

## Stress analysis of Bracket

To simplify analysis, a few assumptions were made. The material selected is titanium, the applied force is 800 lbf, no failure from shear stress, the maximum deflection in any feature has to be less than 0.005 in, the factor of safety is 4, and the mechanics of each feature were simplified for design. However, all analysis was conducted with a safety factor of 5, as I did not initially find the factor of safety in the listed parameters. 

### Feature A

For feature A, it was treated as a cantilever bar with a distributed load. The length of the bar is assumed to be the width of the strap that it supports, which is 0.75in. This leaves the diameter of the bar as the only unknown.
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

### Feature E and Stress Technical Drawings

For feature E, some creativity had to be employed with the stress analysis. The most appropriate and simplified analysis, in my opinion, was to treat it similar to feature A, where it is a cantilever beam with a distributed load. Unlike feature A, the distributed load is the reaction force resulting from contact with the t-beam, and the concentrated support force is the applied force. Similar to feature D, this part is also symmetrical, so analysis was conducted on one side of the feature using half of the total applied force. 
The width of feature E was constrained by the width of feature B on the t-beam, which was 0.9992 in. The depth was once again equal to the length of feature A, which is 0.75 in. This left the height as the only unknown. 
Using the appropriate equations for this loading scenario, the minimum height for E was determined to be 0.365 in.

![comp e and draw](<A5 SoDesignpage0004.jpg>) 

The technical drawings are mostly to scale, as the engineering paper was divided by 0.2 inch grids, simplifying the multi-view drawing. 
Since the bracket is fully defined by the dimensions on the front and side view, no dimensions were included on the top view. 

## Deflection Analysis of Bracket

All of the deflection analysis uses the same assumptions regarding material, deflection, factor of safety, and loading conditions.

### Feature A and B

Unlike in the stress analysis of A, the length of the bar does impact the resulting deflection, so the length of the bar needs to be minimized. Once again, the minimum length is the width of the strap carrying the load, which is 0.75in. 
Using deflection, the minimum diameter was determined to be 0.496in, which is narrower than the resulting stress diameter. 

Since all of the analysis regards deflection, the calculated values in this feature will drive the dimensions in the other features. 
Similar to the stress analysis, the width of B was set to the diameter of A for simplicity, leaving the height and depth unknown. To simplify the equations and minimize deflections, a height of 1 in was selected for feature B.

![Strain a and B](<A5 SoDesignpage0005.jpg>) 

With those assumptions, the only remaining unknown was the depth of feature B. This was determined to be 0.0425 in using the appropriate deflection equations.

### Feature C and D

Since the loading conditions and constraints were already determined in the stress analysis, this simplified the work required for the deflection dimensions.
The length was constrained by the width of the t-beam, which was 2.496 in, and the depth was the length of feature A, 0.75 in.
The height was determined to be 0.478 in.

![comp c and d deflect](<A5 SoDesignpage0006.jpg>)

For feature D, it was once again symmetrically split, and through a simplified axial loading analysis, the wall width was determined to be 0.0210 in. 

### Feature E and Drawings

The only unknown dimension on feature E was the height, as the depth and width were constrained by feature A and the t-beam, respectively. 
The height was calculated at 0.383 in.

![comp e and draw delfect](<A5 SoDesignpage0007.jpg>) 

Similar to the stress bracket, the drawing is mostly to scale due to the grid-lined paper, and the part is fully dimensioned from both calculated and provided values. 

## Follow up and Linkage Analysis

For comparison, the calculated diameter of feature A was chosen. As is seen in the picture, the stress analysis resulted in a larger diameter, meaning that the part would fall outside of the factor of safety from stress rather than exceeding the maximum deflection at any smaller of a size. 
The primary error throughout the document was the usage of a factor of safety of 5 instead of the prescribed 4. This resulted in each individual calculation being incorrect, as well as incorrect calculations stacking upon one another. 
For assumptions, the most likely to be changed is the material selection of titanium. Titanium is stronger than aluminum or steel, so a material change away from titanium would result in larger overall dimensions to account for the extra material required for the same amount of support. The final impact is that the bracket would be both wider and taller.

### Linkage Design
The material was again selected to be titanium, and the linkage assembly is treated as an axially loaded bar to simplify analysis. The length was decided to be 3 in, measured from the centerpoint of one hole to another, and the width of the hole on the top was chosen to be the larger of the 2 previously calculated diameters, 0.634in. The width was set as the maximum width of the bracket, also determined by stress analysis, resulting in a total width of 2.585 in. Since the bracket is symmetrical down the centerline, the effective width of the thinnest section was determined to 0.7925 in. This left depth as the only remaining unknown.
Through stress analysis, the depth was calculated as 0.042 in, whereas it was 0.0398 in using the strain analysis. Since the stress analysis resulted in a larger dimension, that is the one that will be chosen for the final linkage feature. 

![bracket and analysis](<A5 SoDesignpage0008.jpg>)

### Linkage and Feature A Fit

The connection for feature A and the linkage must be a running or sliding fit. From page 651 of the Machinery's Handbook, this was determined to be an RC2 fit. From page 654, the maximum clearance was determined to be 0.00095 in, with a minimum of 0.00025 in. Consulting page 650, this results in a grade 5 standard tolerance. Referencing table 7, again on page 650, the most appropriate and cost effective machining process for this is broaching. 

For the 1 in shaft and the linkage, the fit must be designed for light assembly pressure. The appropriate fit for this is FN1, from page 652, as it is described as light assembly pressure. From table 11 on page 659, the interference of the hole and shaft is between 0.0003 and 0.0012 in. The lowest grade for this fit is grade 8, found from table 6 on page 650, and the most effective machining operations for this fit are reaming and turning. 

Total time for the project ~10 hours. 
