.. _option-CONOPT-method_for_initial_basis:

Method for Initial Basis
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Use slacks away from bounds	



This option sets the method use for creating an initial basis. If the option value equals 'Use slacks away from bounds' (the default), CONOPT uses a procedure similar to the Crash procedures from LP to create an initial basis using structural variables and slacks away from their bounds. Fixed slacks are only included in a last round. If the option setting equals 'Use large infeasible slacks', large infeasible slacks will be included in the initial basis with preference for distance from bound. This setting can be useful combined with the option **Logical Switch for SLP Mode**  set to 'On' if CONOPT uses many iterations in Phase 0.



Possible values are:



    *	Use large infeasible slacks
    *	Use slacks away from bounds




**Learn more about** 

*	:ref:`option-CONOPT-slp_mode`  



