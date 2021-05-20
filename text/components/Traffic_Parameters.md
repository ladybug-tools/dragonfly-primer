## Traffic Parameters

![](../../images/components/Traffic_Parameters.png)

![](../../images/icons/Traffic_Parameters.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Traffic%20Parameters.py)


Create TrafficParameters representing the traffic within an urban area. 



#### Inputs
* ##### watts_per_area [Required]
A number representing the maximum sensible anthropogenic heat flux of the urban area in watts per square meter. This is specifcally the heat that DOES NOT originate from buildings and mostly includes heat from automobiles, street lighting, and human metabolism. If autocalculate, it will be estimated frm the average building story count of the model hosting the traffic parameters (Default: autocalculate). Values for different cities can be found in (Sailor, 2011)[1]. Typical values include: 

    * 20 W/m2 = A typical downtown area

    * 10 W/m2 = A commercial area in Singapore

    * 8 W/m2 = A typical mixed use part of Toulouse, France

    * 4 W/m2 = A residential area in Singapore
* ##### weekday_sch 
A list of 24 fractional values that will be multiplied by the watts_per_area to produce hourly values for heat on the weekday of the simulation. (Default: a typical schedule for a commercial area). 
* ##### saturday_sch 
A list of 24 fractional values that will be multiplied by the watts_per_area to produce hourly values for heat on the Saturday of the simulation. (Default: a typical schedule for a commercial area). 
* ##### sunday_sch 
A list of 24 fractional values that will be multiplied by the watts_per_area to produce hourly values for heat on the Sunday of the simulation. (Default: a typical schedule for a commercial area). 

#### Outputs
* ##### traffic
Traffic parameters that can be plugged into the "DF Assign Model UWG Properties" component to specify the behavior of traffic within an urban area. 