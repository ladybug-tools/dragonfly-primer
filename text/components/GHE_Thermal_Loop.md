## GHE Thermal Loop

![](../../images/components/GHE_Thermal_Loop.png)

![](../../images/icons/GHE_Thermal_Loop.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20GHE%20Thermal%20Loop.py)


Create an Ground Heat Exchanger Loop for a District Energy Simulation (DES) simulation. 

This includes a ground heat exchanger and all thermal connectors needed to connect these objects to Dragonfly Buildings. 



#### Inputs
* ##### ghe_geo [Required]
Horizontal Rhino surfaces representing the footprints of ground heat exchangers. These ground heat exchanging fields contain the boreholes that supply the loop with thermal capacity. Multiple borehole fields can be located along the loop created by the _connector_geo. 
* ##### connector_geo [Required]
An array of lines or polylines representing the thermal connectors within the thermal loop. In order for a given connector to be valid within the loop, each end of the connector must touch either another connector, a building footprint, or a ground heat exchanger. In order for the loop as a whole to be valid, the connectors must form a single continuous loop when passed through the buildings and the heat exchanger field. 
* ##### clockwise 
A boolean to note whether the direction of flow through the loop is clockwise (True) when viewed from above in the GeoJSON or it is counterclockwise (False). (Default: False). 
* ##### borehole 
A GHE BoreholeParameter object from the "DF GHE Borehole Parameters" component, which customizes properties like borehole min/max depth and borehole min/max spacing. 
* ##### soil 
A GHE SoilParameter object from the "DF GHE Soil Parameters" component. This can be used to customize the conductivity and density of the soil as well as the grout that fills the boreholes. 
* ##### fluid 
A GHE Fluid object from the "DF GHE Fluid Parameters" component. This can be used to customize the fuild used (eg. water, glycol) as well as the concentration of the fluid. (Default: 100% Water). 
* ##### pipe 
A GHE Pipe object from the "DF GHE Pipe Parameters" component. This can be used to customize the pipe diameter, conductivty, and roughness. 
* ##### horiz_pipe 
A HorizontalPipe object to specify the properties of the horizontal pipes contained within ThermalConnectors. This can be used to customize the pipe insulation, pressure loss, etc. 
* ##### design 
A GHEDesign object from the "DF GHE Design" component. This can be used to customize the mina and max entering fluid temperatures as well as the max boreholes. 
* ##### name 
Text to be used for the name and identifier of the Thermal Loop. If no name is provided, it will be "unnamed". 
* ##### ghe_names 
An optional list of names that align with the input _ghe_geo and note the name to be used for each ground heat exchanger in the DES loop. If no names are provided, they will be derived from the DES Loop name above. 
* ##### connect_names 
An optional list of names that align with the input _connector_geo and note the name to be used for each thermal connector in the DES loop. If no names are provided, they will be derived from the DES Loop name above. 

#### Outputs
* ##### report
Reports, errors, warnings, etc. 
* ##### des_loop
A Dragonfly Thermal Loop object possessing all infrastructure for a District Energy Simulation (DES) simulation. This should be connected to the loop_ input of the "DF Model to GeoJSON" component. 