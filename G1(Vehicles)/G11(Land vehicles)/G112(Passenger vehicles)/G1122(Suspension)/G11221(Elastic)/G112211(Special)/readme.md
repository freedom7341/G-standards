This standard provides a method of suspension building which totals at less than 25 constraints per four wheeled vehicle (depending on the ballsocket count).<br>
Each wheel will add a minimum of 3 constraints.
Special tools are used which are not common on building servers.
The reason we are using prop engine building tools is to cut down on rope constraints,
usually we would have two ropes representing and acting as two suspension arms which hold the wheel in place.
Here we only have one constraint that holds the wheel in place.
#### Opening note:
All values are purely recommendations.
Everyone does things a little different so you might be keen on using different values, which is completely acceptable.
In this standard I do not insist on using any specific props,
but we will assume that the baseplate does not have collision and that the wheels do.
We will also assume that the building is done parallel to the world's X axis and that the builder is an active user of smart snap.

Before we start, total number of ballsockets can vary. Two reversed ballsockets are stronger than one, four of them is even better.
Elastics can also be multiplied, if one 100k constant elastic isn't enough, add another one.

#### Addons needed:
- Elastic Suspension Tool
- Advanced Ballsocket Tool
- Prop Engine Building Tools
- Smart Snap
- Make Spherical (optional/recommended by even god himself for prop vehicle building)

#### 1. Spawn your wheel prop as well as the base prop which will be used as a chassis.

#### 2. Use make spherical tool on the wheel before you do any constraining.

#### 3. Position your wheel relative to the baseplate.
You will be able to change the height of the wheel later at any point with minimal work.

#### 4. Change the weight of the wheel and baseplate.
Smaller vehicles such as cars tend to have 30-150 units on the wheels and 250-600 on the baseplate, 
remember that a lighter wheel will spin easier than a heavy one.<br>
Bigger vehicles such as trucks use 100-300 units on the wheels and 1000-5000 on the baseplate.

#### 5. Limit the wheel to only move up/down.
Open the "Rope - Slider" tool with these settings:<br>
Width 0.00<br>
Length 50000.00<br>
RopeCount 2<br>
Center 2<br>
- [X] Select third prop
- [ ] Clear objects on holster

Then,<br>
1. Click the baseplate.<br>
2. Click the wheel.<br>
3. Click straight & level ground (world).<br>

Now you have limited the wheel to only move up/down. The height of the wheel dictates the average position, not the position that the vehicle will sit at.
Heavy vehicles will require a lower wheel placement that will then look good only once the vehicle has been unfrozen and is putting weight on the wheels.

#### 6. Ballsocket the wheel.
Open the "Ballsocket - Advanced" tool with these settings:<br>
Force limit	0.00<br>
Torque limit 0.00<br>
X Minimum	-180.00<br>
X Maximum	180.00<br>
Y Minimum	-0.01<br>
Y Maximum	0.01<br>
Z Minimum	-0.01<br>
Z Maximum	0.01<br>
- [X] Free movement
- [ ] No collide entities

Then,<br>
1. Click the center of the wheel side.<br>
2. Click on the side/face of the baseplate which is parallel to the wheel side we clicked on first.<br>

Wheels can be ballsocketed to either the baseplate OR to a rotating plate separated from the vehicle used for steering. DON'T ballsocket to both!

#### 7. Make the elastics.
Open the "ElasticSuspension" tool with these settings:<br>
Elasticity 10000.00 to 100000.00<br>
Damping 2000.00<br>
Relative Damping 1.0
- [ ] StretchOnly

Rope Width doesn't matter<br>
X Offset 0.00<br>
Y Offset 0.00<br>
Z Offset 0.00<br>

Then,<br>
1. Click the wheel (anywhere).<br>
2. Click the baseplate (anywhere).<br>

Elasticity is the constant which affects the elastic, this can be changed to make the suspension stiffer or more relaxed.
The constraint is automatically created in the mass center of the first selected prop which is the wheel.
100k is what i've found to be the upper limit, after 100k there's really no difference in elastic strength.

#### 8. Changing wheel height after building.
1. Open the "ElasticSuspension" tool.<br>
2. Look at the wheel and press R.<br>
3. Move the wheel up or down, preferably with precision.<br>
4. Constrain the wheel again at the new height with the old settings.<br>

This method obviously has to be repeated for every wheel your vehicle might have, they all share the same baseplate so don't get confused.

Wheel spazz is something that has haunted and still haunts all gmod car builders, nowadays to a lesser degree.
It can be easily fixed just by using bigger wheels with a bigger diameter or by using more ballsockets.
It can also be fixed by using Expression 2 chips that manipulate prop inertia.


#### Conclusion.
Suspension Building is the most tedious and most constraint heavy part of vehicle building, however necessary it may be.<br>
This guide shows a method which has the least amount of contraints and entities (looking at you, hydro controllers).
The only simpler method would be to use direct axis center constraints and ballsockets which can't really be called a proper suspension
and does not have the same effect.
