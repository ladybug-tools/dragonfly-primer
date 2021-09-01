# Create EPW

![](../../.gitbook/assets/Create_EPW.png)

![](../../.gitbook/assets/Create_EPW%20%282%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Create%20EPW.py)

Create a custom EPW object from a location and data collections of annual hourly data.

## Inputs

* **location \[Required\]**

  A location object for the epw\_file. 

* **dry\_bulb\_temp**

  Annual hourly data collection for dry bulb temperature \[C\] 

* **dew\_point\_temp**

  Annual hourly data collection for dew point temperature \[C\] 

* **wind\_speed**

  Annual hourly data collection for wind speed \[m/s\] 

* **wind\_direction**

  Annual hourly data collection for wind direction \[degrees\] 

* **direct\_normal\_rad**

  Annual hourly data collection for direct normal radiation \[Wh/m2\] or \[W/m2\] 

* **diffuse\_horiz\_rad**

  Annual hourly data collection for diffuse horizontal radiation \[Wh/m2\] or \[W/m2\] 

* **horiz\_infrared\_rad**

  Annual hourly data collection for horizontal infrared radiation intensity \[Wh/m2\] or \[W/m2\] 

* **direct\_normal\_ill**

  Annual hourly data collection for direct normal illuminance \[lux\] 

* **diffuse\_horiz\_ill**

  Annual hourly data collection for diffuse horizontal illuminance \[lux\] 

* **total\_sky\_cover**

  Annual hourly data collection for the fraction for total sky cover \[tenths\] 

* **atmos\_pressure**

  Annual hourly data collection for weather station pressure \[Pa\] 

* **visibility**

  Annual hourly data collection for visibility \[km\] 

* **ceiling\_height**

  Annual hourly data collection for cloud ceiling height \[m\] 

* **model\_year**

  Annual hourly data collection for the year from which the hourly data has been extracted. This input is necessary when the input data collections are from a leap year. 

* **base\_epw**

  File path to an optional .epw to fill empty slots for data that has not been connected here. 

* **run \[Required\]**

  Set to True to run the component and create the epw\_obj. 

## Outputs

* **report**

  Reports, errors, warnings, etc. 

* **epw\_obj**

  An EPW object that can be written to a file using the Write EPW component. 

