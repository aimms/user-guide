.. _CONOPT_Advanced_-_Method_Finding_Max_Tight_Step:


Method for Finding Maximal Tight Step
=====================================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Standard ratio test method	



This option sets the method used to determine the maximum step during Phase 0 when the tolerances are tightened. If the value of this option equals 'Standard ratio test method', the old method based on the standard ratio test known from LP is used. This is the default value. The method has the advantage that linear constraints that are feasible will remain feasible. If the value equals 'Bending method', a new experimental method is used which is based on bending or projecting the basic variables until the sum of infeasibilities is close to its minimum. The method does not use anti-degeneracy. Cycling is prevented by creating extra large slacks at regular intervals. Note that constraints that initially are feasible may become infeasible due to bending. This applies to both linear and nonlinear constraints.



Possible values are:



*	Standard ratio test method
*	Bending method




**Note** 

*	This option is similar to the option **Method for Finding Maximal Step** , but is applied when tolerances are tightened.




**Learn more about** 

*	:ref:`CONOPT_Advanced_-_Method_Finding_Max_Step` 



