

.. _option-AIMMS-solver_column_row_mapping:


Solver Column Row Mapping
=========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Never	



A column row mapping is a table, which tells which constraint and which variable in the AIMMS model corresponds to which constraint and variable in the solver. Such a map is useful when a solver reports messages about certain constraints and variables, using its internal numbering. The option Solver Column Row Mapping determines when this mapping is reported in the listing file. Possible values are:



    *	Never
    *	At first solve
    *	At an infeasible solve
    *	At every solve



