## Object to String

![](../../images/components/Object_to_String.png)

![](../../images/icons/Object_to_String.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Object%20to%20String.py)


Serialize any dragonfly object to a JSON text string. You can use "DF String to Object" component to load the objects from the file back. 

This includes any Model, Building, Story, Room2D, WindowParameter, or ShadingParameter. 

It also includes any honeybee energy Material, Construction, ConstructionSet, Schedule, Load, ProgramType, or Simulation object. 



#### Inputs
* ##### df_obj [Required]
A Dragonfly object to be serialized to a string. 

#### Outputs
* ##### df_str
A text string that completely describes the honeybee object. This can be serialized back into a honeybee object using the "HB String to Object" coponent. 