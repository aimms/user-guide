.. _ODH-CPLEX_XMIP_Solp_-_Population_Limit:


Population Limit
================



**Type**:	Integer	

**Range**:	{1 .. 2100000000}	

**Default**:	20	



This option limits the number of MIP solutions generated for the solution pool during each call to the populate procedure. Populate stops when it has generated as many solutions as the value of this option. A solution is counted if it is valid for all filters, consistent with the relative and absolute pool gap tolerances, as controlled by the options **Pool Relative Objective Gap**  and **Pool Absolute Objective Gap**  respectively, and has not been rejected by the candidate callback (if any exists), whether or not it improves the objective of the model.



In parallel, populate may not respect this option exactly due to disparities between threads. That is, it may happen that populate stops when it has generated a number of solutions slightly more than or slightly less than this limit because of differences in synchronization between threads.



This option does not apply to MIP optimization generally; it applies only to the populate procedure.



If you are looking for a option to control the number of solutions stored in the solution pool, consider instead the solution pool capacity option **Pool Capacity** .



Populate will stop before it reaches the limit set by this option if it reaches another limit, such as a time limit set by the user. 



This option has only meaning if the option **Do** **Populate**  is switched on.



**Learn more about** 

*	:ref:`ODH-CPLEX_XMIP_Solp_-_Do_Populate`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Abs_Obj_Gap`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Capacity`  
*	:ref:`ODH-CPLEX_XMIP_Solp_-_Pool_Rel_Obj_Gap`  
