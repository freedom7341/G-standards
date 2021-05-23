This standard proposes a method for making hydraulic suspension that can be described as being soft and preferable in off-road vehicles.<br>
It is unique in a way where instead of using the conventional ropes placed in a "V" shape, 
wheels are constrained to a prop block that is axised to the baseplate, working as a suspension arm.<br>

#### 1. Follow the first 5 steps from AV112221(Jackpody) standard.
Get a baseplate and position wheels on it.

#### 2. Spawn 4 props.
Spawn 4 props that are preferably SProps blocks with size of 12x12x36 or 12x12x42.
Freeze them in the air and make sure they are placed in a way where the longest side is parallel to front/rear of the baseplate.
These will work as the suspension arms, imagine them being rods that will connect your wheel to the baseplate and create that up/down only movement.

#### 3. Put the props to inside of wheels.
Place a block's shortest side bottom to the mass center of a wheel in a way where looking from the top,
the block will be poking from the wheel into the baseplate like a stick. Repeat the same for other blocks.

#### 4. Rotate every block.
The blocks are placed parallel to the baseplate, the goal is to angle them from the wheel's mass center upwards about 30-45 degrees.
The blocks should be looking like suspension arms that have let the wheels down. One corner of a block is slightly above the baseplate, while other is in the wheel.

#### 5. Axis the blocks to baseplate.
Using Precision Alignment or other possible tools, create an Axis between block and baseplate around block's bottom shortest side that is above the baseplate.
The axis makes sure the block rotates like an actual suspension arm. Repeat for every block.

#### 6. Constrain front wheels to the blocks.
One way to constrain an object to a prop, but let it rotate freely, is to use ball sockets. But this standard offers using 4 ropes instead of a ball socket,
because ball socket constraints create a bigger air drag penalty on the vehicle. This is called "Rope ball socketing".<br>
If you wish to use ball sockets, you can simply create a ball socket from a wheel to the block, do so for both front wheels.<br>
If you wish to use rope ball sockets, follow these steps:<br>
1. Using precision alignment, create 4 points 50 units above the wheel in an "X" shape so that:
- 1 is to be 50 units forward and to the left (attached to block).
- 2 is to be 50 units forward and to the right (attached to block).
- 3 is to be 50 units to the rear and left (attached to block).
- 4 is to be 50 units to the rear and right (attached to block).
- 5 is to be at the exact center of the prop you and ball and socketing (attached to wheel).
2. Using precision alignment, create four rigid ropes from points 1,2,3,4 to 5.

#### 7. Constrain rear wheels to the blocks.
Since the rear wheels will not be steering, they can be Axis-Centered to their block's directly.

#### 8. Follow steps 8-12 from AV112221(Jackpody) standard.
Spawn a steering E2, wire it.<br>
Make ball sockets, <b>but do not ball socket the rear wheels</b> in step 9, because they are already rotationally constrained to their blocks.<br>
Prepare, make, and adjust the hydraulics.


