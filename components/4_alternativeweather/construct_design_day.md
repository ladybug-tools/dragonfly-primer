# Construct Design Day

![](../../.gitbook/assets/Construct_Design_Day.png)

![](../../.gitbook/assets/Construct_Design_Day%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Construct%20Design%20Day.py)

Construct a design day from a set of parameters.

## Inputs

* **name \[Required\]**

  The name of the DesignDay object. 

* **day\_type \[Required\]**

  Text indicating the type of design day \(ie. 'SummerDesignDay', 'WinterDesignDay' or other EnergyPlus days\). 

* **location \[Required\]**

  A Ladybug Location object describing the location of the design day. 

* **date \[Required\]**

  A Ladybug Date for the day of the year on which the design day occurs. This should be in the format of 'DD Month' \(eg. '1 Jan', '4 Jul'\). The LB Calculate HOY component can also be used to construct this date. 

* **dry\_bulb\_max \[Required\]**

  Maximum dry bulb temperature over the design day \(in C\). 

* **dry\_bulb\_range**

  Dry bulb range over the design day \(in C\). 

* **humidity\_type \[Required\]**

  Type of humidity to use. \(ie. Wetbulb, Dewpoint, HumidityRatio, Enthalpy\) 

* **humidity\_value \[Required\]**

  The value of the humidity condition above. 

* **barometric\_p**

  Barometric pressure in Pa. 

* **wind\_speed \[Required\]**

  Wind speed over the design day in m/s. 

* **wind\_dir \[Required\]**

  Wind direction over the design day in degrees. 

* **sky\_type \[Required\]**

  Type of solar model to use.  \(eg. ASHRAEClearSky, ASHRAETau\) 

* **sky\_properties \[Required\]**

  A list of properties describing the sky above. For ASHRAEClearSky this is a single value for clearness. For ASHRAETau, this is the tau\_beam and tau\_diffuse. 

## Outputs

* **design\_day**

  Script output design\_day. 

