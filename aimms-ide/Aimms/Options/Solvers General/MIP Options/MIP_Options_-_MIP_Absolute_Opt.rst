

.. _Options_MIP_Options_-_MIP_Absolute_Opt:


MIP Absolute Optimality Tolerance
=================================



Type:	Floating point number	

Range:	[0,inf)	

Default:	0



The solution process stops if the solver can guarantee that the current best solution is within MIP Absolute Optimality Tolerance of the global optimum. This is only valid for mixed integer programming models.



**Note** 


*   This option is also valid for MIQP and MIQCP problems.
*   For a MIP, the absolute optimality gap is the absolute value of the difference between the Best Integer Objective (i.e., the incumbent) and the Best Bound (i.e., the objective of the best remaining node).
*   For a MIP, the relative optimality gap is Abs(Best Integer Objective - Best Bound) / (eps + Abs(Best Integer Objective)), where eps is a very small positive constant, i.e., 1e-6.



