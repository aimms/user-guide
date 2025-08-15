

.. _Options_Robust_Optimization_-_Boxed_Ellipsoids:


Boxed Ellipsoids
================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Off	



In case the robust counterpart is a second-order cone program (SOCP), the solver might sometimes face difficulties solving it. To improve convergence properties of the barrier algorithm used by the solver, it sometimes helps to add an enclosing box for each ellipsoid that defines an ellipsoidal uncertainty constraint (or region).



Possible values are:



*	On
*	Off




**Note** 

*	Option **Transform Ellipsoids**  can also be used to improve numerical stability.




**Learn more about** 

*	:ref:`Options_Robust_Optimization_-_Transform_Ellipsoids`  
