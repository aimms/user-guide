.. _option-CPLEX-tuning_measure:


Tuning Measure
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Average	



This option controls the measure for evaluating progress when a suite of models is being tuned. Possible values are:



    *	Average
    *	Minmax




Setting 'Average' uses the mean average of time to compare different option sets over a suite of models. Setting 'Minmax' uses a minmax approach to compare the time of different option sets over a suite of models.





This option is only meaningful if the value of option **Tuning Repeater** is larger than one.





**Learn more about** 

*	:ref:`CPLEX_Tuning_Tool` 
*	:ref:`option-CPLEX-tuning_repeater` 
