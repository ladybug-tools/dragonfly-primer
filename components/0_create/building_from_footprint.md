# Building from Footprint

![](../../.gitbook/assets/Building_from_Footprint.png)

![](../../.gitbook/assets/Building_from_Footprint%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Building%20from%20Footprint.py)

Create Dragonfly Buildings from footprint geometry \(horizontal Rhino surfaces\).

## Inputs

* **footprint\_geo \[Required\]**

  A list of horizontal Rhino surfaces to be converted into Buildings. 

* **floor\_to\_floor \[Required\]**

  A list of float values with a length equal to the number of stories in each Building. Each value in the list represents the floor\_to\_floor height of the Story starting from the first floor and then moving to the top floor. 

* **perim\_offset**

  An optional positive number that will be used to offset the perimeter of the footprint to create core/perimeter Rooms. If this value is None or 0, no offset will occur and each floor plate will be represented with a single Room2D. 

* **name**

  Text to set the base name for the Building, which will also be incorporated into unique Building identifier. This will be combined with the index of each input \_footprint\_geo to yield a unique name for each output Building. If the name is not provided, a random one will be assigned. 

* **program**

  Text for the program of the Buildings \(to be looked up in the ProgramType library\) such as that output from the "HB List Programs" component. This can also be a custom ProgramType object. If no program is input here, the Buildings will have a generic office program. 

* **constr\_set**

  Text for the construction set of the Buildings, which is used to assign all default energy constructions needed to create an energy model. Text should refer to a ConstructionSet within the library such as that output from the "HB List Construction Sets" component. This can also be a custom ConstructionSet object. If nothing is input here, the Buildings will have a generic construction set that is not sensitive to the Buildings's climate or building energy code. 

* **conditioned**

  Boolean to note whether the Buildings have heating and cooling systems. 

* **run \[Required\]**

  Set to True to run the component and create Dragonfly Buildings. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **buildings**

  Dragonfly buildings. 

