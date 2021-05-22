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
