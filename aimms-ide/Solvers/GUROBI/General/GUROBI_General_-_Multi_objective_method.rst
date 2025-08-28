.. _option-GUROBI-multi_objective_method:


Multi Objective Method
======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option determines which algorithm should be used for subsequent solves when solving a continuous multi-objective optimization model. Possible values are:



    *	Automatic
    *	Primal simplex
    *	Dual simplex
    *	Discard warm start




When solving a continuous multi-objective optimization model using a hierarchical approach, the model is solved once for each objective. The algorithm used to solve for the highest priority objective is controlled by the option **Method**. This option determines the algorithm used to solve for subsequent objectives. The default setting 'Automatic' usually chooses primal simplex. The setting 'Discard warm start' indicates that warm-start information from previous solves should be discarded, and the model should be solved from scratch (using the algorithm indicated by the option **Method** ).





**Note** 

*	This option only affects continuous multi-objective models.




**Learn more about** 

*	:ref:`option-GUROBI-method` 
