

.. _Options_NonlinPres_-_Evaluations_Range_Integer_Vari:


Evaluations Range Integer Variables
===================================



:Type:	Integer	
:Range:	{0..:ref:`Miscellaneous_Maxint` }	
:Default:	5	



This option controls whether the AIMMS Presolver will evaluate nonlinear expressions (in a constraint) that contain (bounded) integer variables. Doing so might result in tighter upper and lower bounds for these or other variables.



The value of this option determines which integer variables are used for evaluating nonlinear expressions. If the value of this option equals n > 0, then each integer variable in the model with at most n elements in its range will be used for evaluating nonlinear expressions. For example, if an integer variable has range {0,...,4} (and therefore 5 elements in its range) then it will be used for evaluating nonlinear expressions if this option is set to 5 (the default) but it is excluded if this option is set to 4 (or lower).



If this option is set to 0 then nonlinear expressions will not be evaluated.



**Note** 

*	This option only applies to MINLP and MIQCP models that include constraints with nonlinear expressions containing integer or binary variables.
