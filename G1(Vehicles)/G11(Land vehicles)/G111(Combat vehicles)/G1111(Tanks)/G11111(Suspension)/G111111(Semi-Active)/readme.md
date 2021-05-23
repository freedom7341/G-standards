Semi-Active Suspension by DeHelleman (not for beginners).

#### 1. Setting up your ropes.
1. Select the "Precision Alignment" tool.
2. Select "Mass Centre Point" and make a Point 1 on your wheel.
3. Select "Hitpos Point" and add Points 2, 3 to your baseplate, on the further opposite edges from the wheel.
This basically means the ropes form a "V" shape that reaches out to the side of the baseplate that is opposite to wheels.
4. Press R and go to "Constraints", then select "Rope". Change the "Width" to 0 if you don't want to see your ropes.
5. Making sure the "Rigid" option is checked [X], you select Point 1 on the top list.
6. Now select Point 2 on the bottom list, and click on "Create Constraint", do the same for Point 3.
7. Repeat the process for all wheels.

#### 2. Preparing your hydraulics.
1. Spawn the "Wire Hydraulics" for the wheels, preferably on a separate plate.
2. Spawn as much plates or blocks as there are wheels.
3. Using "Precision Alignment", use "Mass Centre" to move the blocks/plates to the centre of your wheels.
4. When all wheels have their blocks/plates, select the standard "Precision" tool and set "Push/pull amount" to 100.
5. Under the "Push/Pull Amount", uncheck the box that says "Push/pull as percent (%) of target's depth" [ ] and pull/push the blocks/plates of the wheels upwards.
6. Select the "Precision Alignment" tool and select "Mass Centre", 
put a mass centre on your block/plate and then a mass centre on the wheel belonging to the block/plate.
7. Right click your baseplate so it is blue and attach the mass centre point of the block/plate to the baseplate.
8. Now, right click your wire hydraulic controller and press R, then go to "Constraints".
9. Select "Wire Hydraulic" and select Point 1 and Point 2, then "Create constraint".
10. Repeat this process for all wheels, the blocks/plates can be removed upon completion of "Wire Hydraulic" setup.

#### 3. Setting up "Wire Hydraulic" length controller.
1. Spawn a "Constant Value" with the following values:<br>
- 10000 (for constant, can be any value).
- 2000 (for damping, can be any value).
- 200 (for length, should always be 2x your hydraulic length which in this case is 100).
2. Spawn a "Arithmetic-Subtract" gate for each "Wire Hydraulic" controller.
3. Wire all "Subtract" gate "A" to constant value of 200.
4. Wire all "Subtract" gate "B" to its corresponding "Wire Hydraulic" controller's length.
5. Proceed to wire the length from the "Wire Hydraulic" controller's to their corresponding subtract gates.

*Your semi-active suspension by DeHelleman is now complete.*
