.. _CBC_MIP_-_MIP_presolve:


MIP presolve
============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	On	



The MIP presolve algorithm tries to reduce the size of the model in a similar way to the general presolve algorithm (as controlled by option **Presolve** ) and it also tries to strengthen the model. This can be very useful and is worth trying. Possible values are:



*	Off
*	On
*	Clique inequalities
*	SOS
*	Try SOS
*	All inequalities
*	Strategy
*	Aggregate
*	Force SOS




Setting 'Clique inequalities' will turn <= clique constraints into equality constraints. Setting 'SOS' will create SOS sets if all 0-1 in sets (well one extra is allowed) and no overlaps. Setting 'Try SOS' is the same but allows any number extra. Setting 'All inequalities' will turn all valid inequalities into equalities with integer slacks.





**Learn more about** 

*	:ref:`CBC_Presolve_-_Presolve` 
