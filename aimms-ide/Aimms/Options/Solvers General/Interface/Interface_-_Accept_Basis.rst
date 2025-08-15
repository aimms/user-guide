

.. _Options_Interface_-_Accept_Basis:


Accept Basis
============



**Type**:	Floating point number	

**Range**:	[0,1]	

**Default**:	0.01	



After solving a model AIMMS will store the final basis. When this model has to be solved again, after it has been modified, AIMMS can pass the stored basis to the solver. When using this basis as a starting point for solving the modified model, the solver is often faster than if the solver has to start from scratch.



Whether or not AIMMS passes the stored basis to the solver depends on the setting of this option and the effect of your model modifications on the model structure. AIMMS will take the solution of the previous model (corresponding to the stored basis), and determine how many rows in the modified model are infeasible for that solution. If the amount of 'infeasible rows' is too high then AIMMS will not pass the basis (as it is likely that this basis will not be a good starting point for the modified model).



An Accept Basis value of 1 always accepts a provided basis and an Accept Basis of 0 always rejects a basis, even if no changes in the model were made. For other values of Accept Basis, AIMMS will pass the basis if and only if



	number of 'infeasible rows' / number of rows <= Accept Basis.



**Note** 

*	The value of Accept Basis has no influence on the restart basis; the solver will always load the file with the restart basis if the Restart option is set (and the file exists).
*	When you provide your own starting point for a NLP model, which is not the same as the solution of a previous solve of the same model, you should set this option to 0. If you do not do this, it is possible that the NLP solver will not find the optimal solution since the basis might force the solver to search locally while the starting point might not be near the optimal solution.




**Learn more about** 

*   CPLEX:  :ref:`CPLEX_General_-_Restart`
*   COPT:   :ref:`COPT_General_-_Restart`
*   GUROBI: :ref:`GUROBI_General_-_Restart`
*   XA:     :ref:`XA_General_-_Restart`

