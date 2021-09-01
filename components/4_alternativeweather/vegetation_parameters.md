# Vegetation Parameters

![](../../.gitbook/assets/Vegetation_Parameters.png)

![](../../.gitbook/assets/Vegetation_Parameters%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Vegetation%20Parameters.py)

Create VegetationParameters representing the behavior of vegetation within an urban area.

## Inputs

* **albedo**

  A number between 0 and 1 that represents the ratio of reflected radiation from vegetated surfaces to incident radiation upon them. \(Default: 0.25\) 

* **start\_month**

  An integer from 1 to 12 that represents the month at which vegetation evapostranspiration begins \(leaves come out\). By default, the month will be automatically determined by analyzing the epw to see which months have an average monthly temperature above 10C. 

* **end\_month**

  An integer from 1 to 12 that represents the month at which vegetation evapostranspiration ends \(leaves fall off\). By default, the month will be automatically determined by analyzing the epw to see which months have an average monthly temperature above 10C. 

* **tree\_latent**

  A number between 0 and 1 that represents the the fraction of absorbed solar energy by trees that is given off as latent heat \(evapotranspiration\). Currently, this does not affect the moisture balance in the uwg but it will affect the temperature. \(Default: 0.7\). 

* **grass\_latent**

  A number between 0 and 1 that represents the the fraction of absorbed solar energy by grass that is given off as latent heat \(evapotranspiration\). Currently, this does not affect the moisture balance in the uwg but it will affect the temperature. \(Default: 0.5\). 

## Outputs

* **veg\_par**

  Vegetation parameters that can be plugged into the "DF UWG Simulation Parameter" component to specify the behavior of vegetation in the simulation. 

