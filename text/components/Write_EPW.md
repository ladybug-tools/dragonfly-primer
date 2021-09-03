## Write EPW

![](../../images/components/Write_EPW.png)

![](../../images/icons/Write_EPW.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Write%20EPW.py)


Write an EPW object into a .epw file. 



#### Inputs
* ##### epw_obj [Required]
An EPW object such as that exported from the Create EPW component. 
* ##### folder 
A directory into which the .epw file will be written. 
* ##### file_name 
An optional name for the .epw file. Default will use the city of the EPW object's location. 
* ##### run [Required]
Set to True to run the component and write the .epw file. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### epw_file
File path to a .epw that contains all of the data in the input _epw_obj. 