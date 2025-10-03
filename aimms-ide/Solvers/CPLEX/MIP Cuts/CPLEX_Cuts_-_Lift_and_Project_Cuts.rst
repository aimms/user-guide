.. _option-CPLEX-lift_and_project_cuts:


Lift and Project Cuts
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



The value of this option determines if there should be an attempt to generate lift-and-project cuts for the problem.
Setting the value different from 'Off' indicates that the attempt to generate cover cuts should be made. Using the
default indicates that the attempt to generate lift-and-project cuts should continue only if it seems to be helping.
Possible values are:

    *	Off
    *	Automatic
    *	Generate cuts moderately
    *	Generate cuts aggressively
    *	Generate cuts very aggressively

