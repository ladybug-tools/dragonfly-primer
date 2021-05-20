## Search OpenDSS

![](../../images/components/Search_OpenDSS.png)

![](../../images/icons/Search_OpenDSS.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Search%20OpenDSS.py)


Search for available Wires and TransformerProperties within the dragonfly OpenDSS standards library. 



#### Inputs
* ##### keywords 
Optional keywords to be used to narrow down the output list of objects. If nothing is input here, all available objects will be output. 
* ##### join_words 
If False or None, this component will automatically split any strings of multiple keywords (spearated by spaces) into separate keywords for searching. This results in a greater liklihood of finding an item in the search but it may not be appropropriate for all cases. You may want to set it to True when you are searching for a specific phrase that includes spaces. (Default: False). 

#### Outputs
* ##### transformers
A list of all transformer properties within the dragonfly OpenDSS standards library (filtered by keywords_ if they are input). 
* ##### wires
A list of all wires within the dragonfly OpenDSS standards library (filtered by keywords_ if they are input). 