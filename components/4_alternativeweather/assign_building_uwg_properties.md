# Assign Building UWG Properties

![](../../.gitbook/assets/Assign_Building_UWG_Properties.png)

![](../../.gitbook/assets/Assign_Building_UWG_Properties%20%281%29.png) - [\[source code\]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Assign%20Building%20UWG%20Properties.py)

Edit the properties of a Dragonfly Building that affect simulation with to the Urban Weather Generator \(UWG\).

## Inputs

* **building \[Required\]**

  A Dragonfly Building which is to have its Urban Weather Generator \(UWG\) properties assigned. 

* **program**

  Text for the name of the building program. Must be one of the options below. \(Default: LargeOffice\).

  * LargeOffice
  * MediumOffice
  * SmallOffice
  * MidriseApartment
  * Retail
  * StripMall
  * PrimarySchool
  * SecondarySchool
  * SmallHotel
  * LargeHotel
  * Hospital
  * Outpatient
  * Warehouse
  * SuperMarket
  * FullServiceRestaurant
  * QuickServiceRestaurant

* **vintage**

  Text for the vintage of the building. This will be used to set default constructions. Must be one of the options below or one of the options from the "HB Building Vintages" component, which will be mapped to one of the options below. \(Default: New\).

  * New
  * 1980\_Present
  * Pre1980

* **fr\_canyon**

  A number from 0 to 1 that represents the fraction of the building's waste heat from air conditioning that gets rejected into the urban canyon. \(Default: 0.5\). 

* **shgc**

  A number from 0 to 1 that represents the SHGC of the building's windows. This is used to evaluate the amount of solar heat reflected into the street canyon. By default, it will be set by the building vintage and the Model climate zone. 

* **wall\_alb**

  A number from 0 to 1 that represents the exterior wall albedo of the building. By default, it will be set by the building program and the DoE commercial reference buildings. 

* **roof\_alb**

  A number from 0 to 1 that represents the exterior roof albedo of the building. By default, it will be set by the vintage, meaning 0.7 for New and 0.2 for 1980\_Present and Pre1980. 

* **roof\_veg**

  A number from 0 to 1 that represents the fraction of the building's roofs covered in vegetation. \(Default: 0\). 

## Outputs

* **report**

  ... 

* **building**

  The input Dragonfly Building with its UWG properties re-assigned based on the input. 

