### These are the rules for how standards should be structurally organized.

#### 1. Avtomat standards begin with AV, sub-groups are separated by the "-" symbol.
An example of how standards are organized:
* AV-1 (Transportation)
  * AV-1-1 (Land vehicles)
    * AV-1-1-1 (Combat vehicles)
    * AV-1-1-2 (Passenger vehicles)
    * AV-1-1-X
  * AV-1-2 (Air vehicles)
  * AV-1-X
* AV-X

#### 2. There must be exactly one "readme.md" file in every sub-directory explaining the principles of how to do a certain thing.
This is done to make this repository more readable, contents of files named "readme.md" automatically appear to users who are in the directory without opening it.
If you want to share your knowledge on how to build light vehicle bodies with props, you would put your description in:
 * AV-X (Transportation)
   * AV-X-X (Land vehicles)
     * AV-X-X-X (Passenger vehicles)
       * AV-X-X-X-X (Exterior)
         * readme.md

#### 3. If there comes a situation where two standards provide different methods for same topic, they are separated into sub-branches.
For example, car suspension can be built with hydraulics or elastics. These are two different methods for same task, 
hence why they should be in two different sub-branches.

#### 4. Every standard has a short, understandable name.
The name of the standard should be in the context of its parent-branch. Example:<br>
Hydraulic suspension standard is a child of the branch *AV-X-X-X (Suspension)*<br>
The hydraulic suspension standard should be named *AV-X-X-X-X (Hydraulic)*.<br> 
A <b>wrong</b> name would be *AV-X-X-X-X (Land vehicle hydraulic suspension)*.<br>
This is done to avoid long names.
