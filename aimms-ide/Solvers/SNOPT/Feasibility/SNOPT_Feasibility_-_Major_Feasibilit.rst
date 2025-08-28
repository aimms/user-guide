.. _option-SNOPT-major_feasibility_tolerance:


Major Feasibility Tolerance
===========================



:Type:	Floating point number	
:Range:	[0,1000]	
:Default:	1e-6	



This option specifies how accurately the nonlinear constraints should be satisfied. The default value of 1e-6 is appropriate when the linear and nonlinear constraints contain data to about that accuracy. SNOPT requires that the maximum nonlinear constraint violation, normalized by the size of the solution plus 1, is smaller than or equal to the **Major Feasibility Tolerance** .



If some of the problem functions are known to be of low accuracy, a larger value of this option may be appropriate.



