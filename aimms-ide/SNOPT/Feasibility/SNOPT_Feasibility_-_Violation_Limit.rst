.. _SNOPT_Feasibility_-_Violation_Limit:


Violation Limit
===============



**Type**:	Floating point number	

**Range**:	[0,1e20]	

**Default**:	10.0	



This option defines an absolute limit on the magnitude of the maximum constraint violations after the line search. Let t be the value of this option. On completion of the line search, the new iteration point xk+1 satisfies the condition



vi(xk+1) <= t max { 1, vi(x0) },



where x0 is the point at which the nonlinear constraints are first evaluated and vi(x) is the ith nonlinear constraint violation vi(x0) = max{ 0, li – Fi(x), Fi(x) – ui }.



The effect of this violation limit is to restrict the iteration points to lie in an expanded feasible region whose size depends on the magnitude of tt. This makes it possible to keep the iteration points within a region where the objective is expected to be well-defined and bounded below. If the objective is bounded below for all values of the variables, then the value of this option may be any large positive value.



