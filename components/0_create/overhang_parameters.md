# Overhang Parameters

![](../../.gitbook/assets/Overhang_Parameters.png)

![](../../.gitbook/assets/Overhang_Parameters%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Overhang%20Parameters.py)

Create Dragonfly shading parameters with instructions for a single overhang \(awning, balcony, etc.\) over an entire wall.

## Inputs

* **depth \[Required\]**

  A number for the overhang depth. 

* **angle**

  A number for the for an angle to rotate the overhang in degrees. Default is 0 for no rotation. 

## Outputs

* **shd\_par**

  Shading Parameters that can be applied to a Dragonfly object using the "DF Apply Facade Parameters" component. 

