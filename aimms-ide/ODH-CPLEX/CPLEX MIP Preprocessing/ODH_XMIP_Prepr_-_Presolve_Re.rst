.. _option-ODHCPLEX-presolve_relaxed_mip:


Presolve Relaxed MIP
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



When this option is switched on, the CPLEX Presolve will be invoked for linear programs for the initial relaxation of a MIP, according to the other presolve option settings. Sometimes additional reductions can be made beyond any MIP presolve reductions that may have already been done. At the default setting CPLEX decides. Possible values are:



*	Automatic
*	Off
*	On



