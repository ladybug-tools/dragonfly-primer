# Color Room2D Attributes

![](../../.gitbook/assets/Color_Room2D_Attributes.png)

![](../../.gitbook/assets/Color_Room2D_Attributes%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Color%20Room2D%20Attributes.py)

Color Dragonfly Room2Ds in the Rhino scene using their attributes.

This can be used as a means to check that correct properties are assigned to different Room2Ds.

## Inputs

* **df\_obj \[Required\]**

  A Dragonfly Model, Building, Story or Room2D to be colored with their attributes in the Rhino scene. 

* **attribute \[Required\]**

  Text for the name of the Room2D attribute by which the Room2Ds should be separated. The "DF Room2D Attributes" component lists all of the attributes of the Room2D. 

* **legend\_par**

  An optional LegendParameter object to change the display of the colored Room2Ds. \(Default: None\). 

## Outputs

* **mesh**

  Meshes of the Room2D floors colored according to their attributes. 

* **legend**

  Geometry representing the legend for colored meshes. 

* **wire\_frame**

  A list of lines representing the outlines of the rooms. 

* **values**

  A list of values that align with the input Room2Ds noting the attribute assigned to each Room2D. 

* **colors**

  A list of colors that align with the input Room2Ds, noting the color of each Room2D in the Rhino scene. This can be used in conjunction with the native Grasshopper "Custom Preview" component and other dragonfly visualization components \(like "DF Visulaize All"\) to create custom visualizations in the Rhino scene. 

