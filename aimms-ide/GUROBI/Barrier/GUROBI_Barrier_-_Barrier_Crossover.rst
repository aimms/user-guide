.. _option-GUROBI-barrier_crossover:


Barrier Crossover
=================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines the crossover strategy used to transform the barrier solution into a basic solution. Use value 'Off' to disable crossover; the solver will return an interior solution. Other options control whether the crossover algorithm tries to push primal or dual variables to bounds first, and then which simplex algorithm is used once variable pushing is complete. Possible values are:



*	Automatic
*	Off
*	Dual first + primal simplex
*	Dual first + dual simplex
*	Primal first + primal simplex
*	Primal first + dual simplex




Options 'Dual first + primal simplex' and 'Dual first + dual simplex' push dual variables first, then primal variables. Option 'Dual first + primal simplex' finishes with primal, while option 'Dual first + dual simplex' finishes with dual.





Options 'Primal first + primal simplex' and 'Primal first + dual simplex' push primal variables first, then dual variables. Option 'Primal first + primal simplex' finishes with primal, while option 'Primal first + dual simplex' finishes with dual. The default value of 'Automatic' chooses automatically.




