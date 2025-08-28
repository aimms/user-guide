.. _option-KNITRO-feasible_mode:


Feasible Mode
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	


This option indicates whether or not the feasible version of Knitro should be used. Possible values are:

    *	Off
    *	On


Given an initial point which sufficiently satisfies all inequality constraints as defined by,


.. math::

   cl + tol \leq c(x) leq cu - tol


(for :math:`cl \ne cu`), the feasible version of Knitro ensures that all subsequent solution estimates strictly satisfy
the inequality constraints. However, the iterates may not be feasible with respect to the equality constraints.
The tolerance :math:`tol > 0` for determining when the feasible mode is active is determined by the option
**Feasible Mode Activation Tolerance**. To enter feasible mode, the point given to Knitro must be strictly
feasible with respect to the inequality constraints. If the initial point is infeasible (or not sufficiently
feasible according to the above formula) with respect to the inequality constraints, then Knitro will run the
infeasible version until a point is obtained which sufficiently satisfies all the inequality constraints.
At this point it will switch to feasible mode.

This option and the option **Honor Bounds** may be useful in applications where functions are undefined outside
the region defined by inequalities.


**Note** 

*	This option can only be used with the interior-point optimizers.


**Learn more about** 

*	:ref:`option-KNITRO-feasible_mode_activation_tolerance`  
*	:ref:`option-KNITRO-honor_bounds`  
