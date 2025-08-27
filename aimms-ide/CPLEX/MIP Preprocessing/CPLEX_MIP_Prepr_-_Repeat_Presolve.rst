.. _option-CPLEX-repeat_presolve:


Repeat Presolve
===============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option lets you tell CPLEX to re-apply the MIP presolve techniques of the presolver to a MIP model at the root after preprocessing has otherwise finished (that is, after cut generation at the root). Possible values are:



    *	Automatic
    *	Off
    *	Repeat without cuts
    *	Repeat with cuts
    *	Repeat with cuts and new root cuts



