## Simple Window Ratio Parameters

![](../../images/components/Simple_Window_Ratio_Parameters.png)

![](../../images/icons/Simple_Window_Ratio_Parameters.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Simple%20Window%20Ratio%20Parameters.py)


Create Dragonfly window parameters with instructions for a single window using an area ratio with the base surface. 



#### Inputs
* ##### ratio [Required]
A number between 0 and 1 for the ratio between the window area and the parent wall surface area. 

#### Outputs
* ##### win_par
Window Parameters that can be applied to a Dragonfly object using the "DF Apply Facade Parameters" component. 