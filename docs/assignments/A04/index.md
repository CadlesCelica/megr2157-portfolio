# A4 – [Topic]

## Objective


## Analyze


## Decide


## Communicate

## CAD
To start, a base of 28x28mm was constructed. This was inspired by other motor mount designs, and leaves no overhang of the motor itself.

This works, as the minimum required width of the beam from the calculations is 15.4mm. Additionally, one hole for the shaft is added, with a nominal value of 6mm. The screw holes for the motor are then added, with a nominal clearance of 3.4mm

The first feature is then extruded 4.5mm up from the top plane. This is so that the keyway portion of the motor shaft is exposed, and the solid shaft passes through the beam, and so that the boss of the motor sits flush with the mount. 

For the second feature, it retains the same width as the first feature, being 28mm. The height is 94.6mm, determined from the maximum possible height of the motor from its tolerances. 

Using beam bending and deflection equations with the given force of 300N and a calculated lever arm of 2.5mm equal to the depth of material at the boss of the motor, the minimum depth of the part is 1.86mm. This comes from the maximum stress equation, as it produced a higher value than the deflection equation.

Assuming the bracket mount holes need to be the same clearance as the motor screw holes, 4 are added with a hole diamater of 3.4mm







