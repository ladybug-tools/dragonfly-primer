## Apply Facade Parameters

![](../../images/components/Apply_Facade_Parameters.png)

![](../../images/icons/Apply_Facade_Parameters.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Apply%20Facade%20Parameters.py)


Apply WindowParameters and/or ShadingParameters to any Dragonfly object (Building, Story, Room2D). 



#### Inputs
* ##### df_obj [Required]
A Dragonfly Building, Story or Room2D which will have the input WindowParameters and/or ShadingParameters assigned to it. 
* ##### win_par 
A WindowParameter object that dictates how the window geometries will be generated for each of the walls. If None, the window parameters will remain unchanged across the input object. If an array of values are input here, different WindowParameters will be assigned based on cardinal direction, starting with north and moving clockwise. 
* ##### shd_par 
A ShadingParameter objects that dictate how the shade geometries will be generated for each of the walls. If None, the shading parameters will remain unchanged across the input object. If an array of values are input here, different ShadingParameters will be assigned based on cardinal direction, starting with north and moving clockwise. 

#### Outputs
* ##### report
The execution information, as output and error streams 
* ##### df_obj
The input Dragonfly object with the WindowParameters and/or ShadingParameters assigned to it. 