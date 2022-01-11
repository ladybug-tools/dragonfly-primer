## Model To Honeybee

![](../../images/components/Model_To_Honeybee.png)

![](../../images/icons/Model_To_Honeybee.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Model%20To%20Honeybee.py)


Convert a Dragonfly Model into a series of Honeybee Models. 



#### Inputs
* ##### model [Required]
A Dragonfly Model object. 
* ##### obj_per_model 
Text to describe how the input Buildings should be divided across the output Models. Default: 'Building'. Choose from the following options: 

    * District - All buildings will be added to a single Honeybee Model.Such a Model can take a long time to simulate so this is only recommended for small numbers of buildings. 

    * Building - Each building will be exported into its own Model.For each Model, the other buildings input to this component will appear as context shade geometry. 

    * Story - Each Story of each Building will be exported into itsown Model. For each Honeybee Model, the other input Buildings will appear as context shade geometry as will all of the other stories of the same building. 
* ##### use_multiplier 
If True, the multipliers on each Building's Stories will be passed along to the generated Honeybee Room objects, indicating the simulation will be run once for each unique room and then results will be multiplied. If False, full geometry objects will be written for each and every story in the building such that all resulting multipliers will be 1. (Default: True). 
* ##### add_plenum 
Boolean to indicate whether ceiling/floor plenums should be auto-generated for the Rooms. The height of ceiling plenums will be autocalculated as the difference between the Room2D ceiling height and Story ceiling height. The height of the floor plenum will be autocalculated as the difference between the Room2D floor height and Story floor height. (Default: False). 
* ##### ceil_adjacency 
Boolean to note whether adjacencies should be solved between interior stories when Room2Ds perfectly match one another in their floor plate. This ensures that Surface boundary conditions are used instead of Adiabatic ones. Note that this input has no effect when the _obj_per_model_ is Story. (Default: False). 
* ##### cap_shades 
Boolean to note whether building shade representations should be capped with a top face. Usually, this is not necessary to account for blocked sun and is only needed when it's important to account for reflected sun off of roofs. (Default: False). 
* ##### shade_dist 
An optional number to note the distance beyond which other buildings' shade should not be exported into a given Model. This is helpful for reducing the simulation run time of each Model when other connected buildings are too far away to have a meaningful impact on the results. If None, all other buildings will be included as context shade in each and every Model. Set to 0 to exclude all neighboring buildings from the resulting models. Default: None. 
* ##### run [Required]
Set to "True" to have the Dragonfly Model translated to a series of Honeybee Models. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### hb_models
Honeybee Model objects derived from the input _models. These Models are ready to be simulated in either an Energy or Radiance simulation or they can be edited further with the Honeybee components. 