# Deconstruct Object

![](../../.gitbook/assets/Deconstruct_Object.png)

![](../../.gitbook/assets/Deconstruct_Object%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Deconstruct%20Object.py)

Deconstruct any Dragonfly geometry object into its unique constituent Dragonfly objects.

This is useful for editing auto-generated child objects separately from their parent. For example, if you want to assign all of the ground floors of a given auto-generated Building to have a Retail ProgramType, this can give you all of such Stories. Then you can assign a Retail ProgramType to them and combine them with the other Stories into a new Building.

## Inputs

* **df\_obj \[Required\]**

  A Dragonfly Building, Story or Room2D to be deconstructed into its constituent objects. Note that, Room2Ds do not have sub-objects assigned to them and the original object will be output. 

## Outputs

* **stories**

  The unique Story objects that make up the input \_df\_obj. This includes unique Stories that make up input Buildings as well as any input orphaned Stories. 

* **room2ds**

  The unique Room2D objects that make up the input \_df\_obj. This includes any unique Room2Ds assigned to input Stories or Buildings as well as any input orphaned Room2Ds. 

