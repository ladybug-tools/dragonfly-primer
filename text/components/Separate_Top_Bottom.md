## Separate Top Bottom

![](../../images/components/Separate_Top_Bottom.png)

![](../../images/icons/Separate_Top_Bottom.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Separate%20Top%20Bottom.py)


Separate the top and bottom floors of a Building into unique Stories with a multiplier of 1 and automatically assign the first story Room2Ds to have a ground contact floor and the top story Room2Ds to have an outdoor-exposed roof. 

This is particularly helpful when trying to account for the heat exchange of the top or bottom floors with the gound or outdoors. 



#### Inputs
* ##### buildings [Required]
Dragonfly Building objects which will have their top and bottom stories separated into unique ones with a multiplier of 1. This can also be an entire Dragonfly Model. 
* ##### sep_mid 
Boolean to note whether all mid-level Stories with non-unity multipliers should be separated into two or three Stories. This means that the top of each unique story will have outdoor-exposed roofs when no Room2Ds are sensed above a given room. (Default: False). 

#### Outputs
* ##### buildings
The Building objects with their top and bottom floors separated. 