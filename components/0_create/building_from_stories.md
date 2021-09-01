# Building from Stories

![](../../.gitbook/assets/Building_from_Stories.png)

![](../../.gitbook/assets/Building_from_Stories%20%282%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Building%20from%20Stories.py)

Create a Dragonfly Building from individual Dragonfly Story objects.

## Inputs

* **stories \[Required\]**

  A list of Dragonfly Story objects to be joined into one Building. 

* **multipliers**

  An optional list of integers with the same length as the input \_stories, which will be used to override any existing multipliers on the input Story objects. This integer denotes the number of times that each Story is repeated over the height of the building. If nothing is input here, the multipliers on the existing Story objects will remain. 

* **name**

  Text to set the name for the Building, which will also be incorporated into unique Building identifier. If the name is not provided a random one will be assigned. 

* **constr\_set**

  Text for the construction set of the Building, which is used to assign all default energy constructions needed to create an energy model. Text should refer to a ConstructionSet within the library such as that output from the "HB List Construction Sets" component. This can also be a custom ConstructionSet object. If nothing is input here, the Building will have a generic construction set that is not sensitive to the Buildings's climate or building energy code. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **building**

  Dragonfly Building. 

