# String to Object

![](../../.gitbook/assets/String_to_Object.png)

![](../../.gitbook/assets/String_to_Object%20%282%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20String%20to%20Object.py)

Serialize any dragonfly JSON text string back to a dragonfly object.

This includes any Model, Building, Story, Room2D, WindowParameter, or ShadingParameter.

It also includes any dragonfly energy Material, Construction, ConstructionSet, Schedule, Load, ProgramType, or Simulation object.

## Inputs

* **df\_str \[Required\]**

  A text string that completely describes the dragonfly object. 

## Outputs

* **df\_obj**

  A Dragonfly object serialized from the input string. 

