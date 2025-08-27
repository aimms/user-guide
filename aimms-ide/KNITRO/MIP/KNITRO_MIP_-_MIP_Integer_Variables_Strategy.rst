.. _option-KNITRO-mip_integer_variables_strategy:


MIP Integer Variables Strategy
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	None	



This option specifies how Knitro should handle integer variables. Possible values are:



    *	None
    *	Relax
    *	MPEC




Setting 'None' means that no special treatment is applied.





Setting 'Relax' implies that all integer variables are relaxed.





Setting 'MPEC' implies that all binary variables are converted to complementarity constraints.

