

.. _Baron_Logging_-_Pass_model_names:


Pass model names
================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Off	



If this option is turned on, the AIMMS names of the variables and constraints are used in the model file when passing the model to BARON. If this option is turned off, the variables are passed as x0, x1, x2, etc, and the constraints as e1, e2, e3, etc. Possible values are:



*	Off
*	On




**Note** 

*	If the AIMMS names are passed, the characters '(' (left parenthesis), ')' (right parenthesis), ',' (comma), '-' (minus sign), ' ' (space), '/' (slash), '\' (backslash), '&' (ampersand) and '.' (dot) are replaced by '_' (underscore) in the model file. For example, ``'Inventory(stock1,period19)'`` will be passed as ``'Inventory_stock1_period19_'``.
*	The characters '<', '=' and '>' are passed as 'l', 'e' and 'g' respectively.
*	Non English letters like 'é', 'ò' and 'á' are passed as 'e', 'o' and 'a' respectively.




**Learn more about** 

*	:ref:`Baron_Logging_-_Keep_model_file` 



