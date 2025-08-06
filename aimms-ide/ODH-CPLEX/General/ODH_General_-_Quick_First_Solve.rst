.. _ODH-CPLEX_General_-_Quick_First_Solve:


Quick First Solve
=================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	No	



This option influences the acceleration of the initial CPLEX solve. Possible values are:



*	No
*	Yes




If set to 'No', the initial solve is not accelerated if presolve is set applied to the full model (as controlled by the option **Presolve** ).





If set to 'Yes', the existing presolved model is used.





**Learn more about** 

*	:ref:`ODH-CPLEX_General_-_Presolve`  



