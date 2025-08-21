.. _option-CONOPT-method_for_defined_variables:


Method for Defined Variables
============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Initial point	



This option specifies the method when defined variables are identified. Defined variables are identified from constraints of the type x(i) = f(x) where x(i) is free or implied free. Possible values are:



*	Initial point
*	Kept basic




If this option equals 'Initial point' then defined variables are only used in the initial point and for the initial basis.





If this option equals 'Kept basic' then defined variables are kept basic and the defining constraints are used to recursively assign values to the defined variables in all trial points.




