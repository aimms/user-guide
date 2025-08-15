.. _CPLEX_Benders_-_Benders_Decomposition_Check_Limit:


Benders Decomposition Check Limit
=================================



**Type**:	Integer	

**Range**:	{0 .. 2100000000}	

**Default**:	10



This option specifies how much detailed information AIMMS should print when CPLEX concludes that the Benders decomposition, as specified by the user, is invalid.



If this option is set to 0 then no detailed information will be printed. Otherwise the following checks are done:




*   check whether each variable has a valid decomposition value, that is, a nonnegative value for continuous variables and a value of 0 for integer variables.
*   check whether each constraint contains variables that all have the same decomposition value or a decomposition value of 0.



This option limits the number of lines that will be printed for each of these two checks. At the default value at most 2*10 = 20 lines are printed.



The information will be printed in the Messages Window.



**Remark** 

The information is also written to the file 'CPLEX 22.1.sta' if the general solvers option **Solver Listing Messages**  is set to a value unequal to 'Never'. 
The file 'CPLEX 22.1.sta' is placed in the log directory of the AIMMS project.

Of course, the ``22.1`` in the filename will be replaced by the actual CPLEX version number.


**Learn more about** 

*	:ref:`CPLEX_Benders_-_Benders_Strategy` 
*	:ref:`Options_Solver_Specific_-_Solver_List1` 



