.. _CPLEX_MIP_Solp_-_Populate_time_limit:


Populate Time Limit
===================



**Type** :	Integer	

**Range** :	{0 .. 2100000000}	

**Default** :	2100000000	



This option sets a time limit on the second phase of the populate algorithm. If the value is set to 0 then the second phase will be skipped (but still the solutions generated during the first phase will be added to the solution pool).



The general time limit, as controlled by the general solvers option **Time Limit** , sets a time limit for the complete populate algorithm, i.e., the first and second phase combined. If this time limit is hit during the first phase of the populate algorithm then the second phase will be skipped. In that case the solver status will be 'Resource Interrupt'. If either one of time limits is hit during the second phase, the solver status will be 'Normal Completion' (since then an optimal solution is found during the first phase).



This option has only meaning if the option **Do** **Populate**  is switched on.



**Learn more about** 

*	:ref:`CPLEX_MIP_Solp_-_Do_Populate`  
*	:ref:`Options_Stop_Criteria_-_Time_Limit`  
