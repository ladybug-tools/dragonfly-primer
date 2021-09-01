# Substation

![](../../.gitbook/assets/Substation.png)

![](../../.gitbook/assets/Substation%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Substation.py)

Create an OpenDSS Substation from its footprint geometry \(horizontal Rhino surfaces\).

## Inputs

* **geo \[Required\]**

  A horizontal Rhino surface representing a footprint to be converted into a Substation. 

* **name**

  Text to set the name for the Substation, which will also be incorporated into unique Substation identifier.  If the name is not provided, a random one will be assigned. 

## Outputs

* **substation**

  A Dragonfly Substation object that can be used within an Electrical Network. 

