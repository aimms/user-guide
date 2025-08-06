.. _ODH-CPLEX_XGeneral_-_Conflict_Algorithm:


Conflict Algorithm
==================



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option can be used to choose the algorithm CPLEX uses in the conflict refiner, in case the general solvers option **Infeasibility Finder**  is switched on. Possible values are:



*	Automatic
*	Fast
*	Propagate
*	Presolve
*	IIS
*	Limited solve
*	Full solve




The algorithm selected by default by CPLEX ordinarily yields the fastest possible performance. However, in certain models, a nondefault selection can work better. In particular, settings 'Fast', 'Propagate', or 'Presolve' entail preprocessing or propagation algorithms that are very fast, but those same algorithms can be inefficient at discarding large numbers of constraints quickly. In such a case, explicitly setting this parameter to 'Limited solve' for a limited solve by the conflict refiner or 'Full solve' for a full solve can improve performance.





Setting 'IIS' invokes the conflict refiner to detect an irreducibly inconsistent set (IIS) in a linear program (LP). You can apply this setting anyway to models that are not strictly LP; in that case, CPLEX tries to detect a conflict using only the linear constraints of the model.





**Learn more about** 

*	:ref:`Options_Solution_-_Infeasibility_Finde`  
