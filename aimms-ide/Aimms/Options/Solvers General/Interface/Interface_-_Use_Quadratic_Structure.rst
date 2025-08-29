

.. _option-AIMMS-use_quadratic_structure:


Use Quadratic Structure
=======================

:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	


This option is currently used only by the solver :ref:`SolverKnitro`. Possible values are:

    *	Off
    *	On
    *	Automatic


When this option is turned on, quadratic terms of the objective function and the constraints are passed to the
solver using special API functions for quadratic structure. If this option is turned off, the quadratic terms
are treated as nonlinear terms.

With the default setting ("Automatic") this option is on for QP, QCP, MIQP, and MIQCP model types. For all
other model types, this option is off in the automatic mode.

