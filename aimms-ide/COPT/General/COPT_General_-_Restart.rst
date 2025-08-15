.. _COPT_General_-_Restart:

Restart
=======



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	No	



In some cases one might want to interrupt the current solve and continue it later on. In order to restart the solver, essential information about the current solution should be saved in a file. Furthermore, the solver should be told to read this data and continue the solve. This option can be used to generate the necessary restart information and to restart the solver. Possible values are:



*	Before
*	No (do not restart)
*	Yes (restart)




Restart files are named coptddddd.mst (MIP start file) for MIP and coptddddd.bas (basis file) for LP. The number ddddd represents the current value of the option **Restart File Number** .





When this option is set to "Yes" then COPT will restart a problem if the restart file exists. In that case the restart file is loaded just before the solve.





This option also determines whether a restart file is written. If this option is set to "Yes" then COPT will write a restart file after the solve. If this option is set to "Before" then COPT will write a restart file before the solve. Writing a restart file before the solve only makes sense if a solution has been passed to COPT. For MIP problems this means that the option **MIP Start**  should be switched on.





**Learn more about** 

*	:ref:`COPT_MIP_-_MIP_start` 
*	:ref:`COPT_General_-_Restart_file_number` 
