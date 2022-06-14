## Validate Model

![](../../images/components/Validate_Model.png)

![](../../images/icons/Validate_Model.png) - [[source code]](https://github.com/ladybug-tools/dragonfly-grasshopper/blob/master/dragonfly_grasshopper/src//DF%20Validate%20Model.py)


Get a validation report that contains a summary of all issues with the Model. 

This includes checks for basic properties like adjacency as well as geometry checks. 



#### Inputs
* ##### model [Required]
A Dragonfly Model object to be validated. This can also be the file path to a Model DFJSON that will be validated. 
* ##### validate [Required]
Set to "True" to validate the the Model and get a report of all issues with the model. 

#### Outputs
* ##### report
A report summarizing any issues with the input _model. If anything is invalid about the input model, this component will give a warning and this report will contain information about the specific parts of the model that are invalid. Otherwise, this report will simply say that the input model is valid. 