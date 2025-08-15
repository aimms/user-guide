.. _GUROBI_Presolve_-_Linearize_Quadratic_Constraint:


Linearize Quadratic Constraints
===============================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic



This option controls presolve Q matrix linearization. Possible values are:



*	Automatic
*	Off
*	Strong relaxation
*	Compact relaxation




Settings 'Strong relaxation' and 'Compact relaxation' attempt to linearize quadratic constraints or a quadratic objective, potentially transforming an MIQP or MIQCP model into an MIP. Option 'Strong relaxation' focuses on getting a strong LP relaxation while option 'Compact relaxation' aims for a compact relaxation. Option 'Off' shuts off the transformation. The default setting chooses automatically. The automatic setting works well, but there are cases where forcing Q linearization can be beneficial.

