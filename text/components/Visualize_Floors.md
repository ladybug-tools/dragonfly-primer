## Visualize Floors

![](../../images/components/Visualize_Floors.png)

![](../../images/icons/Visualize_Floors.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Visualize%20Floors.py)


Preview any Dragonfly geometry object as floor plates within the Rhino scene, including all stories represented by multipliers 



#### Inputs
* ##### df_objs [Required]
A Dragonfly Model, Building, Story, Room2D, or ContextShade to be previewed as a list of floor plates in the Rhino scene. 

#### Outputs
* ##### geo
The Rhino version of the Dragonfly geometry object, which will be visible in the Rhino scene. 