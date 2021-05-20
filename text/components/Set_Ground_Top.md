## Set Ground Top

![](../../images/components/Set_Ground_Top.png)

![](../../images/icons/Set_Ground_Top.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Set%20Ground%20Top.py)


Set Room2Ds or Stories to have their floor in contact with the ground or their roofs in contact with the outdoors. 



#### Inputs
* ##### df_obj [Required]
Dragonfly Stories or Room2Ds which will have its floor set to be in contact with the ground or its roof to be in contact with the outdoors. 
* ##### grnd_contact 
A boolean noting whether the input objects have floors in contact with the ground. 
* ##### top_exposed 
A boolean noting whether the input objects have ceilings exposed to the outdoors. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### df_obj
The input Dragonfly object with its ground_contact or top_exposed properties edited. 