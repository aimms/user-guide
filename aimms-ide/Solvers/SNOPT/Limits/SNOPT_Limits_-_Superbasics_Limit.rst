.. _option-SNOPT-superbasics_limit:


Superbasics Limit
=================



:Type:	Integer	
:Range:	{-1..1000000}	
:Default:	-1	



This option places a limit on the storage allocated for superbasic variables. Ideally, the value of this options should be set slightly larger than the "number of degrees of freedom" expected at an optimal solution.



The default value of -1 is special; in that case the superbasics limit is set equal to the number of nonlinear variables plus 1.



For linear programs, an optimum is normally a basic solution with no degrees of freedom. (The number of variables lying strictly between their bounds is no more than the number of general constraints.)



Normally, the value of this option does not need to be greater than the number of nonlinear variables plus 1. For many problems, the value of this option may be considerably smaller than the number of nonlinear variables. This will save storage if there are many nonlinear variables.



For nonlinear programs, the number of degrees of freedom is often called the "number of independent variables".



