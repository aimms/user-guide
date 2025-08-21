.. _option-CPLEX-barrier_always:


Barrier Always
==============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



Setting this option to "Yes" will cause every barrier optimization run to be started afresh. In case of the default setting, only the initial solve of the linear model will be performed afresh, whereas each solve of the updated versions of the model will use information gathered during the previous solves. This implies that in case of the barrier-crossover solver, the simplex solver will be used to solve the updated model in most cases. Possible values are:



*	No (do not start each barrier optimization run afresh)
*	Yes (do start each barrier optimization run afresh)



