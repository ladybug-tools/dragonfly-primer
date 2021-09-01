# Geometry Properties

![](../../.gitbook/assets/Geometry_Properties.png)

![](../../.gitbook/assets/Geometry_Properties%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Geometry%20Properties.py)

Get properties of any Dragonfly geometry object.

## Inputs

* **df\_objs \[Required\]**

  A Dragonfly Model, Building, Story or Room2D for which properties will be output. 

## Outputs

* **height**

  For a Model or a Building, this will be the average height of the object above the ground. For a Story, this will be the floor-to-floor height and, for a Room2D, this will be the floor-to-ceiling height. 

* **floor\_area**

  A number for the floor area  of all Rooms in the dragonfly object. 

* **ext\_wall\_area**

  A number for the total area of walls in the dragonfly object with an Outdoors boundary condition. 

* **ext\_win\_area**

  A number for the total area of windows in the dragonfly object with an Outdoors boundary condition. 

* **volume**

  A number for the volume of all Rooms in the dragonfly object. 

