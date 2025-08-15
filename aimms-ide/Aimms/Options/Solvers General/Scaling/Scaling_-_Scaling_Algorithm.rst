

.. _Options_Scaling_-_Scaling_Algorithm:


Scaling Algorithm
=================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option controls the algorithm used by AIMMS to scale the model before sending it to the solver. Possible values are:



*	Automatic
*	Iterative
*	Optimization based
*	Combination




The Iterative algorithm first scales the constraints and then the variables. This process is repeated during several iterations. This algorithm finds scaling factors for individual columns and rows. For example, if the model contains the variable X(i), with i in {1,...,5}, then the scaling factor found for X(1) might be different than the one found for X(2). Only linear variables and constraints are scaled.





The Optimization based algorithm solves an MIP model to determine the scaling factors. This algorithm is also used by the :ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model`  inside the Math Program Inspector. This algorithm finds scaling factors at the symbolic level, that is, it will find scaling factors for variables and constraints. For example, it will return the same scaling factor for all X(i), so the scaling factor for X(1) will be equal to that of X(2) to X(5).





The Combination algorithm will first apply the Optimization based algorithm and use the scaling factors found by this algorithm as a "hot start" to apply the Iterative algorithm. The Combination algorithm finds scaling factors for individual columns and rows just as the Iterative algorithm.





The Iterative algorithm is available for linear and nonlinear models. The Optimization based algorithm and the Combination algorithm are only available for linear models.





At the 'Automatic' setting AIMMS will select the Iterative algorithm for a nonlinear model. For a linear model AIMMS will use the Combination algorithm but it will check the scaling score after the first step with the Optimization based algorithm; if the scaling score is below a certain threshold value (currently 500) then the second step with the Iterative algorithm will be skipped. (The scaling score is explained in the help of the option **Scale Model** .)





**Note** 

*	This option is only used if the option **Scale Model**  has been switched on.
*	AIMMS does not scale constraint programming models nor models with complementarity constraints. Scaling is also not applied to stochastic models, the robust counterpart of a model and the dual of a model.
*	The option**List Scaling Factors**  can be used to list the scaling factors, as found by the scaling algorithm, that are used in the scaled model.




**Learn more about** 

*	:ref:`Options_Scaling_-_List_Scaling_Factors` 
*	:ref:`Options_Scaling_-_Scale_Model` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model` 



