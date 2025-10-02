.. _option-CPLEX-restart:


Restart
=======



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



In some cases one might want to interrupt the current solve and continue it later on. In order to restart the solver,
essential information about the current solution should be saved in a file. Furthermore, the solver should be told to
read this data and continue the solve. This option can be used to generate the necessary restart information and to
restart the solver.

When this option is set to 'Yes', the solver will restart a problem if the solution file cpx\ *ddddd*\ .sol exists. The
number *ddddd* represents the current value of the option **Restart File Number**. After the solve the file
cpx\ *ddddd*\ .sol will be generated. Possible values are:

    *	No
    *	Yes


**Learn more about** 

*	:ref:`option-CPLEX-restart_file_number` 

