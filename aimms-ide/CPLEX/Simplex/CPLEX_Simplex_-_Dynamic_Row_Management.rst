.. _option-CPLEX-dynamic_row_management:


Dynamic Row Management
======================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	Automatic	



This option specifies how CPLEX should manage rows in the current model during dual simplex optimization. More specifically, this option controls the use of the kernel simplex method (KSM) for the dual simplex algorithm. That is, CPLEX dynamically adjusts the dimensions of the basis matrix during execution of the dual simplex algorithm, according to the settings of this option. Possible values are:



    *	Automatic
    *	Keep all rows
    *	Manage rows




When the value of this option is 'Automatic', its default value, this option specifies that the user wants CPLEX to manage rows dynamically, adjusting the dimensions of the basis matrix during dual simplex optimization. When it is set to 'Keep all rows', this option specifies that CPLEX must keep all rows. When it is set to 'Manage rows', this option specifies that CPLEX can keep or discard rows according to its internal calculations.




