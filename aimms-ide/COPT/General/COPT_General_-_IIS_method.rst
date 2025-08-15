.. _COPT_General_-_IIS_method:


IIS Method
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines which method to use when calculating an Irreducible Inconsistent Subsystem (IIS). An IIS is a subset of the constraints and variable bounds of the original model. If all constraints in the model except those in the IIS are removed, the model is still infeasible. However, further removing any one member of the IIS produces a feasible result. Possible values are:



*	Automatic
*	Small
*	Fast




Method 'Fast' is often faster than method 'Small' while method 'Small' can produce a smaller IIS.

