.. _option-CPOPT-dynamic_probing:


Dynamic probing
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls probing carried out during search. Probing can be useful on some problems as it can make stronger inferences on combinations of constraints. Possible values for this parameter are 'On' (dynamic probing is activated with a constant strength), 'Automatic' (dynamic probing is activated and its strength is adjusted adaptively) and 'Off' (dynamic probing is deactivated). Possible values are:



*	Automatic
*	Off
*	On




The strength of probing can be defined by option **Dynamic Probing Strength** . Dynamic probing only has an effect if option **Search Type**  equals 'Restart', on problems without interval variables.





**Learn more about** 

*	:ref:`option-CPOPT-dynamic_probing_strength` 
*	:ref:`option-CPOPT-search_type` 
