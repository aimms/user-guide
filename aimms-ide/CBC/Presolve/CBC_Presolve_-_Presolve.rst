.. _option-CBC-presolve:


Presolve
========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option controls the presolve level. Presolve analyzes the model to find such things as redundant equations, equations which fix some variables, equations which can be transformed into bounds etc. For the initial solve of any problem this is worth doing unless you know that it will have no effect. Setting 'On' will normally do 5 passes while using setting 'More' will do 10. Possible values are:



    *	Off
    *	On
    *	More




**Learn more about** 

*	:ref:`option-CBC-presolve_tolerance`  






