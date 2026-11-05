# A9 – Pulleys, Belts, and Bearings

## Objective
Given a static tension, pulley diameter, center distance, rotational speed, belt material, yield strength, and factor of safety, an appropriate belt, shaft, and bearing must be decided through engineering principles. 

## Belt Calculations

First, the belt diameter and length must be determined. 
The given parameters are: The belt does not slip, Tension is 6 lbf static, the system operates at 2000 rpm, pulley diameter of 2 in, a safety factor of 3, the pulley is steel, the belt has a yield strength of 471 psi at 20% yield and is made of polyurethane rubber, and the center distance is 6 in.

The static belt length, inner diameter, is calculated from 2x the center distance + the diameter of the pulley. From this, the belt is calculated to be 21.4 in. Since the belt is in a 20% stretched state, the unstretched length of the belt is determined to be 17.85 in, inner diameter.

![img 1](<A9 Doc_page-0001.jpg>)

For the next step, the stress in the belt must be calculated. 
From the lecture, the coefficient of static friction between polyurethane rubber and steel is 0.6, so this value was used in the dynamic equation. Combining with the static equations, F1 is determined to be 10.42 lbf, and F2 is 1.58 lbf. From the allowable stress and the larger applied force F1, the diameter is calculated to be 0.29 in. In standard sizes and appropriate lengths, the appropriate belt diameter is 3/8 in. The total outer diameter is calculated to be 20.2 in. This corresponds to part # 3044K608, 20.25 in belt. 

ss of belt listing

## Shaft Calculations

Using the power transmission of the pulley, and knowing there is no slip, the shaft must transmit the same power, which is 0.044 hp. 

![img 2](<A9 Doc_page-0002.jpg>)

Using equations from the Machinery's Handbook, and adjusting for the specific material, the minimum diameter with a factor of safety of 3 is calculated at 0.149 in. In standard American sizes, the closest shaft is 3/16 in. 


## Bearing Calculations

The force supported by the bearing is found from the equation F1 + F2 = 2F, where 2F is the reaction force at each pulley. This force is 12 lbf.

![img 3](<A9 Doc_page-0003.jpg>)

Using the shaft diameter and belt diameter as the projected area, the P, V, and PV are calculated. Using the calculated values, porous bronze is an appropriate bearing material for this application. 

ss of bearing

## Frame

For the frame, the height was set to 3x the shaft diameter, for a total h = 0.5625 in. The depth was initially calculated for the factor of safety, assuming the bar is axially loaded. 

![img 4](<A9 Doc_page-0004.jpg>)

Upon further reflection, the part would need to be 3/8 in thick to accomodate the bearing length. The factor of safety was recalculated, and determined to be 943.

## Lessons 




