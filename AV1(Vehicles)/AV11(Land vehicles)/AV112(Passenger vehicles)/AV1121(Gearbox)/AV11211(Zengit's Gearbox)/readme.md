Your ACF vehicle might be powerful, but a lot of its potential can be lost due to improperly adjusted gears.
They might be too short and you reach your top speed too early, or they might be too long and you overload your engine.
Another common mistake is that the whole power band of an engine is not used.
This standard proposes a gear tuning method for ACF vehicles to achieve their maximum top speed with biggest acceleration.

#### 1. Test ground.
First you must find a drag strip with enough runway, such as the gm_carcon_ws one.
You can use other maps too, just make sure there is a long straight where you will be able to reach the maximum speed of your vehicle due to air drag.

#### 2. Make differential ratios 1.
Before you do any adjusting, update your differentials to have gear ratios and final drives equal to 1,
this will help make the calculations easier in future. You can leave the gearbox final drive on 0.5, which is probably the most optimal.

#### 3. Adjust gears so it is drivable.
Once you have updated all your final drives to 1, the car will probably be very sluggish.
You must now decrease all the gear ratios so the car accelerates at all.
Try run it to the end of drag strip with full RPM in each gear and see if you can reach the last gear.
If not, decrease the gears again.

#### 4. Find the top gear.
Now that your car accelerates decently enough, your aim is to find the perfect gear ratio of the last gear.
Take a look at your engine and check for the power band.
For example, an engine has a power band 5750-8500 RPM and gearbox has 5 gears.
Every car with air drag will have some kind of a maximum top speed,
your goal is to adjust the last gear so the car stops accelerating almost exactly at end of power band, in example case 8500 RPM. <br>

Example of action:
1) The 5th gear is set to 0.37 and top speed is reached at 7500 RPM. This means the 5th gear ratio must be smaller, for example 0.33.
2) The 5th gear is set to 0.33 and top speed is reached at 8900 RPM. This means the 5th gear ratio must be bigger, for example 0.34.
3) The 5th gear is set to 0.34 and top speed is reached at 8600 RPM, which is almost ideal.
4) The 5th gear is set to 0.35 and top speed is reached at 8400 RPM, this leaves room for error in case somehow top speed is increased.
It can now be determined that the best ratio for last gear is 0.35 in given case.

#### 5. Calculate the other gears.
Now that you have found the perfect last gear, you can calculate all the other gears.
You must now get a power band ratio. In example case power band is 5750-8500, so the power band ratio (PBR) is:<br>
*PBR = 5750 / 8500 = 0.676*<br>
This is the theoretical perfect, but drivers may fail to switch gears perfectly every single time, so the value must be rounded up to, for example,
0.7 to account for that.

Other gears are calculated follows:<br>
5th gear = 0.35 (from before)<br>
4th gear = 0.35 * 0.7 = 0.245 ~ 0.25 (It is best to round these values up)<br>
3rd gear = 0.25 * 0.7 = 0.175 ~ 0.18<br>
2nd gear = 0.18 * 0.7 = 0.126 ~ 0.13<br>
1st gear = 0.13 * 0.7 = 0.091 ~ 0.10<br>

The calculated gearbox follows this pattern:<br>
1: 0.10<br>
2: 0.13<br>
3: 0.18<br>
4: 0.25<br>
5: 0.35<br>

Gear ratios like these make sure when you switch to next gear at maximum power band RPM, your RPM will drop to the minimum power band RPM.
This makes sure you accelerate to your top speed by using the entire engine power band.

#### 6. Adjust gear placement.
If you did exactly as shown, chances are your 1st and 2nd gears will feel very short and useless.
In this case you can simply remove the shorter gears and move gears downwards.

In the case you wish to remove the first 2 gears, the gearbox would look something like this:<br>
1: ~~0.10~~ 0.18<br>
2: ~~0.13~~ 0.25<br>
3: ~~0.18~~ 0.35<br>
4: ~~0.25~~ 0.40 (These are overdrive gears and don't matter, you can put whatever you want here) <br>
5: ~~0.35~~ 0.45<br>

Generally you want your 1st gear not to make excessive wheel-spin, but also to not overload the engine.
Every car will be different - some will need all 5 gears, some will need only 2 for top speed.
The reverse gear can be set to 0.01 bigger than the 1st gear, but it has no significance.<br>
The example gearbox would look like this:<br>
1: 0.18<br>
2: 0.25<br>
3: 0.35<br>
4: 0.40<br>
5: 0.45<br>
R: -0.19<br>
FD: 0.5<br>

#### Conclusion.
Generally you want to tune your gears when you know the car will not change its weight or any other properties.
If you want to change the final drive, you have to recalculate all the gear ratios from start.


