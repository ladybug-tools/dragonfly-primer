## Write DDY

![](../../images/components/Write_DDY.png)

![](../../images/icons/Write_DDY.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Write%20DDY.py)


Write Ladybug DesignDays to a standard .ddy file. 



#### Inputs
* ##### location [Required]
A Ladybug Location object describing the location data in the weather file. 
* ##### design_days [Required]
A list of DesignDay objects representing the design days contained within the ddy file. 
* ##### folder 
An optional folder to save the .ddy file. 
* ##### name 
An optional name for this .ddy file. 
* ##### run [Required]
Set to "True" to run the component and write the .ddy file. 

#### Outputs
* ##### ddy_file
A .ddy file path that has been written to your system. 