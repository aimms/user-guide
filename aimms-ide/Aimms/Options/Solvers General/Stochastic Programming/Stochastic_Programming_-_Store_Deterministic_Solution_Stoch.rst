

.. _option-AIMMS-store_deterministic_solution_as_stochastic:


Store Deterministic Solution as Stochastic
==========================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



This option determines, for a stochastic model, whether AIMMS should store the solution of non-stochastic (or deterministic) variables in the .Stochastic suffix or the .Level suffix. Possible values are:



    *	Off
    *	On




If this option is set to 'On' (the default) then the .Stochastic suffix will be used otherwise the .Level suffix.





If this option is set to 'On' then the solution of the underlying deterministic model remains completely intact after solving the stochastic model, as the solution of a stochastic model is entirely stored in the .Stochastic suffix. This will not be the case if this option is set to 'Off'.




