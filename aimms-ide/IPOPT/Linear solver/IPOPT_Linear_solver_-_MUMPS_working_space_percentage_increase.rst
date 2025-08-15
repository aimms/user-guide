

.. _IPOPT_Linear_solver_-_MUMPS_working_space_percentage_increase:


MUMPS working space percentage increase
=======================================



:Type:	Integer	
:Range:	{0..2147483647}	
:Default:	1000	



This option specifies the percentage increase in the estimated working space for MUMPS. In MUMPS, when significant extra fill-in is caused by numerical pivoting, larger values for this option may help use the workspace more efficiently. On the other hand, if memory requirements are too large at the very beginning of the optimization, choosing a much smaller value for this option, such as 5, might reduce memory requirements.



**Note** 

*	This option is only used if the option **Linear Solver Selection**  has been set to 'MUMPS solver'. 




**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
