# Deconstruct All Object

![](../../.gitbook/assets/Deconstruct_All_Object.png)

![](../../.gitbook/assets/Deconstruct_All_Object%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Deconstruct%20All%20Object.py)

Deconstruct any Dragonfly geometry object into ALL of its constituent Dragonfly objects.

This is useful for editing auto-generated child objects separately from their parent. For example, if you want to assign all of the ground floors of a given auto-generated Building to have a Retail ProgramType, this can give you all of such Stories. Then you can assign a Retail ProgramType to them and combine them with the other Stories into a new Building.

## Inputs

* **df\_obj \[Required\]**

  A Dragonfly Building, Story or Room2D to be deconstructed into all of its constituent objects. Note that, Room2Ds do not have sub-objects assigned to them and the original object will be output. 

## Outputs

* **all\_stories**

  Script variable Python 

* **all\_room2ds**

  Script variable Python 

