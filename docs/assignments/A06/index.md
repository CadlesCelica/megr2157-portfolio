# A6 – [Engineering Drawings and Parametric Modelling]
## Feature A

Since many of the calculations were completed within A5, most of the work consisted of creating variables and equations to properly parametrically model the bracket.

Many of the universal variables were established in feature A, and were referenced in future features. This includes the yield strength, factor of safety, load on each side of the strap, length of the bar, corrected yield strength, and the equation required to find the diameter. 

![test test test](<EQN A.png>)
![test test test](<dim diam A.png>)
![test test test](<extrude A.png>)  

For both the sketch and feature, all dimensions are defined parametrically to allow easy modification should it be necessary. This is also true for all of the features. 

For clarification, see assignment A5.

## Feature B

For this feature and additional features, only additional variables and equations are shown.
If units of length are not specified, they are all in inches.

![Eqn B](<Var feat B.png>)
 ![sketch b](<Sketch B.png>) 
![extrude B](<Extrude B.png>)

## Feature C

![eqn C](<Var feat C.png>) 
![sketch C](<sketch C.png>) 
![ext C](<extrude C.png>)


## Feature D

![eqn d](<Var D.png>)
![sketch d](<sketch D.png>) 
![ext d](<Feat D.png>) 
![mirror d](<feat d mirror.png>) 

## Feature E

![eqn e](<var E.png>)
![sketch e](<sketch E.png>) 
![ext e](<feat E.png>) 
![mirror e](<feat E mirror.png>) 

## Final Part and Drawing

![final part](<part final.png>)
![final draw](<draw ss edit.png>)

For the tolerance block, only relevant tolerances are included. This is why there is no 0.1in tolerance, angular, or fractional tolerance. 
The fit tolerances are seperately called out.

## Lessons Learned
### Part A
 Since the stress equations resulted in larger dimensions throughout the part, they drove the dimensions for each individual feature. For feature A, the equation was expressed in terms of the defined variables applied load, corrected yield strength, and length of the bar, and the cube root was taken to find the diameter. This was the most difficult to define, as Solidworks only has a built in square root function, so some trial and error was experienced to generate the proper output. 

### Part B
 For feature D, a tighter tolerance was required, as it directly affects one of the surfaces required for the part C fit on the T beam. The tolerance for this part was determined from the appropriate fit found in the Machinery's Handbook. For many of the other parts, the default tolerances were applied. Since not all of these dimensions are critical to the strength of the feature, this will unnecessarily increase cost and time to machine, especially since the selected material is titanium. 


## Link

### Final Reflections
Tolerancing for part compatibility was fascinating, as many of the tolerances required for various fit types were a lot tighter than I expected. Before referencing the tables, I assumed tolerances for fits would be in the thousandths of an inch at the smallest, but this was not the case. Many of the fits required tolerances in the ten-thousandths of an inch, leading to overall clearance in the thousandths of an inch. 

By defining some parts to have a tighter tolerance than others, this directly correlates to the importance of each dimension. The tolerances required for a fit are critical, as they inferface with other parts and must work correctly. Alternatively, less critical measurements, such as overall length, are less important as they do not directly interface with other parts, and are allowed to have a larger overall tolerance. The smaller the tolerance, the more critical the feature is to the intended design of the part.

## Parts Download
All of the parts can be found for download [HERE test](https://github.com/CadlesCelica/megr2157-portfolio/blob/edd20f299af98818a4262a3b1203257e8825edcd/docs/assignments/A06/SLDW%20files)