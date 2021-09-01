# Separate Top Bottom

![](../../.gitbook/assets/Separate_Top_Bottom.png)

![](../../.gitbook/assets/Separate_Top_Bottom%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Separate%20Top%20Bottom.py)

Separate the top and bottom floors of a Building into unique Stories with a multiplier of 1 and automatically assign the first story Room2Ds to have a ground contact floor and the top story Room2Ds to have an outdoor-exposed roof.

This is particularly helpful when using to\_honeybee workflows with multipliers but one wants to account for the heat exchange of the top or bottom floors with the gound or outdoors.

## Inputs

* **buildings \[Required\]**

  Dragonfly Building objects which will have their top and bottom stories separated into unique ones with a multiplier of 1. 

## Outputs

* **buildings**

  The Building objects with their top and bottom floors separated. 

