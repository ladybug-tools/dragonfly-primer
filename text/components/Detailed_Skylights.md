## Detailed Skylights

![](../../images/components/Detailed_Skylights.png)

![](../../images/icons/Detailed_Skylights.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Detailed%20Skylights.py)


Add detailed skylight geometries to Dragonfly Room2Ds. 



#### Inputs
* ##### df_objs [Required]
A Dragonfly Model, Building, Story or Room2D, to which the _windows should be added. 
* ##### skylights [Required]
A list of Breps that will be added to the input _df_objs as detailed skylights. 

#### Outputs
* ##### df_objs
The input dragonfly objects with the input _windows added to it. 