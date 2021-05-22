### If you feel like there is something that is missing in the given standards, feel free to define a new standard, we are open to contributions from anyone!
#### You can contribute by creating a pull request or messaging owners of this repository directly.
#### You can also contribute by correcting spelling mistakes, grammar and nuances of other people's standards, no contribution is useless.

### There are certain rules you must follow to contribute:

#### 1. Classify your standard accordingly.
It is important to have a standard in the correct sub-branch. If you are unsure where your standard should be, feel free to contact the owners of this repository!

#### 2. There must be one "readme.md" file in every sub-directory explaining the principles of how to do a certain thing.
This is done to make this repository more readable, contents of files named "readme.md" automatically appear to users who are in the directory without opening it.
If you want to share your knowledge on how to build light vehicle bodies with props, you would put your description in:
 * AV-X (Transportation)
   * AV-X-X (Land vehicles)
     * AV-X-X-X (Passenger vehicles)
       * AV-X-X-X-X (Exterior)
         * readme.md

Where you would describe some fundamental steps on how to build a vehicle body.

#### 3. Include an explanation of your standard.
Make sure to include some kind of an explanation on what the reader is about to follow, otherwise the steps may seem confusing out of context.

#### 4. Standards must be written in a step-by-step style with numbering.
Example of a bad standard:<br>
*To make a setang, simply get this E2 (E2 code) and spawn a gate, then ballsocket your wheels to the setang and ballsocket setang to wheels.*

Example of a good standard:<br>
*1. Create an E2 gate by using this E2 code (E2 code).*<br>
*2. Wire the "Baseplate:entity" of E2 to your baseplate.*<br>
*3. Make sure your wheels, baseplate and E2 are aligned to the world.*<br>
*4. Configure the "ballsocket-advanced" tool to have these values: (values).*<br>
*5. ...*<br>

#### 5. Split explanations into smaller directories.
Try not to write 100 lines of text in one standard if otherwise impossible. Splitting up your ideas and explanations will make it easier to read and reference a standard for others.<br>
If there comes a situation where two people want to share different methods for same work, the standards are put into separate sub-branches.
