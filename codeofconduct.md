### These are the rules for how standards should be structurally organized.

#### 1. Avtomat standards begin with AV, every group under a branch is numbered from 1 to 9.
If there happens to be more than 9 sub-branches of one branch, alphabetical letters are used.
An example of how standards are organized and written:
* AV1(Transportation)
  * AV11(Land vehicles)
    * AV111(Combat vehicles)
    * AV112(Passenger vehicles)
    * AV113
    * AV114
    * AV115
    * AV116
    * AV117
    * AV118
    * AV119
    * AV11A
    * AV11B
    * AV11C
  * AV12(Air vehicles)
  * AV13
* AV2(Tools)

#### 2. There must be exactly one "readme.md" file in every sub-directory explaining the principles of how to do a certain thing.
This is done to make this repository more readable, contents of files named "readme.md" automatically appear to users who are in the directory without opening it.
If you want to share your knowledge on how to build light vehicle bodies with props, you would put your description in:
 * AVX(Transportation)
   * AVXX(Land vehicles)
     * AVXXX(Passenger vehicles)
       * AVXXXX(Exterior)
         * readme.md

#### 3. If there comes a situation where two standards provide different methods for same topic, they are separated into sub-branches.
For example, car suspension can be built with hydraulics or elastics. These are two different methods for same task, 
hence why they should be in two different sub-branches.

#### 4. Every standard has a short, understandable name.
The name of the standard should be in the context of its parent-branch. Example:<br>
Hydraulic suspension standard is a child of the branch *AVXXX(Suspension)*<br>
The hydraulic suspension standard should be named *AVXXXX(Hydraulic)*.<br> 
A <b>wrong</b> name would be *AVXXXX(Land vehicle hydraulic suspension)*.<br>
This is done to avoid long names.

#### 5. Standard formatting.
5.1. Every standard must use the same syntax.<br>
5.2. In the beginning of each standard, an introduction is given as to what the method is, preferably its benefits and unique features are mentioned.
Introduction text is plain and without styling.<br>
5.3. Every step is numbered and given a short name or sentence, ending with a period symbol.<br>
5.4. Every step is marked as a heading by including four hashtags, space, and the step number, for example:<br>
"#### 3. Adjust parameters."<br>


