## Solve Adjacency

![](../../images/components/Solve_Adjacency.png)

![](../../images/icons/Solve_Adjacency.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Solve%20Adjacency.py)


Solve adjacencies between the Room2Ds of Dragonfly objects. 



#### Inputs
* ##### df_objs [Required]
A list of dragonfly Room2Ds for which adjacencies will be solved. This can also be Dragonfly Stories, Buildings or an entire Model, in which case each Story will have adjacencies solved across its Room2Ds. 
* ##### adiabatic 
Set to True to have all the discovered wall adjacencies set to an adiabatic boundary condition. If False, a Surface boundary condition will be used for all adjacencies. Note that adabatic conditions are not allowed if interior windows are assigned to interior walls. (Default: False). 
* ##### air_boundary 
Set to True to have all the discovered wall adjacencies set to an AirBoundary type. Note that AirBoundary types are not allowed if interior windows are assigned to interior walls. (Default: False). 
* ##### no_overwrite 
Boolean to note whether existing Surface boundary conditions should be preserved while solving adjacencies. If True, no intersection will occur and only newly-discovered adjacencies will be updated. If False or unspecified, all geometry will be cleaned and intersected before solving adjacencies. In either case, existing windows will be preserved. 
Note that, to make use of this option effectively, Room2Ds must already have matching edge segments in order for them to be discovered as adjacent. The "DF Intersect Room2Ds" component can be used to ensure adjacent rooms have matching segments without changing any boundary conditions. (Default: False). 
* ##### run [Required]
Set to True to run the component and solve adjacencies. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### df_objs
The input Dragonfly objects with adjacencies solved between the Room2D wall segments. 