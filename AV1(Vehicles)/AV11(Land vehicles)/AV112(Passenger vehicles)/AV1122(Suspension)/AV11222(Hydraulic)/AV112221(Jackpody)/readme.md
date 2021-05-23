This standard explains how to build simple Jackpody's suspension with hydraulics for lightweight cars.<br>
The primary idea of Jackpody's suspension is to use hydraulics that are attached from a wheel to a point some distance upwards.<br>
It is based on Jackpody's video: https://www.youtube.com/watch?v=Flex-2so_Zs

#### 1. Spawn a baseplate for your car.
Preferably you want to use SProps.

#### 2. Always build suspension while the car's front is facing north of the map.
You can figure out where north is by putting down your spray on the ground - the spray's up will be the map's north.

#### 3. Find a wheel.
Preferably a SProps wheel 25-35, but you can use anything you like. Spawn 4 wheels and freeze them in the air, so they are aligned with north.

#### 4. Make spherical.
Use the "Make Spherical" tool on all 4 wheels.

#### 5. Place the wheels on the baseplate where you want them to be.
Preferably use the "Precision Alignment" or "Precision" tool.

#### 6. Create ropes.
There are multiple ways you can create ropes, usually it resembles a "V" shape, where bottom of V is the mass center of the wheel, 
and both upper corners of "V" are points attached to the baseplate.<br>
The "V" shape limits the wheel's travel to up/down only.

#### 7. Make sure everything is aligned to world.
You can use the "Precision" tool to make sure props are aligned to world exactly, this plays a key role in precision.

#### 8. Spawn a steering E2.
This is when you can spawn your E2 for steering, it is needed to create ball-sockets.
Make sure to wire the steering E2 to your baseplate before you make ball-sockets.
#### 9. Make ball-sockets.
The most common approach is to use the "Ball-Socket Advanced" tool two ways by flipping the limits of Y and Z axis.<br>
Set your "Ball-Socket Advanced" tool to have these settings:<br>
X minimum: -180.00<br>
X maximum: 180.00<br>
Y minimum: <b>-0.01</b><br>
Y maximum: <b>0.01</b><br>
Z minimum: <b>-0.01</b><br>
Z maximum: <b>0.01</b><br>
- [X] Free Movement<br>

"No-Collide Entities" is optional, all other values are 0.<br>

Then, create ball-sockets:<br>
1. From rear wheels to baseplate.
2. From front wheels to E2 steering.

Then, inverse the Y and Z axis such that:<br>
Y minimum: <b>0.01</b><br>
Y maximum: <b>-0.01</b><br>
Z minimum: <b>0.01</b><br>
Z maximum: <b>-0.01</b><br>

Then, create ball-sockets:<br>
1. From baseplate to rear wheels.<br>
2. From E2 steering to front wheels.<br>

#### 10. Prepare points for hydraulics.
The point for wire hydraulic can be set using a prop or specific "Precision Alignment" functions.
In Jackpody's suspension the point is usually set 30-48 units above the wheel,
and maybe 6-12 units to the inside of the car to prevent wheels popping too easily.

#### 11. Make hydraulics.
Make the wire hydraulics and, preferably, put their controllers on a seperate prop.

#### 12. Adjust hydraulics.
You can then change the wire hydraulic length, constant and damping values.<br>
As a rule of thumb, if the car acts very unstable and wants to shake, damping is too high.
