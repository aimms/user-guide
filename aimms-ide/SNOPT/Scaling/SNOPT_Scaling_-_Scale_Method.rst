.. _SNOPT_Scaling_-_Scale_Method:


Scale Method
============



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option determines which method is used for scaling. The setting 'No scaling' is recommended if it is known that x and the constraint matrix never have very large elements (say, larger than 1000). With setting 'Only scale linear rows and columns' the constraints and variables are scaled by an iterative procedure that attempts to make the matrix coefficients as close as possible to 1.0. This will sometimes improve the performance of the solution procedures. With setting 'Additional scaling' the constraints and variables are scaled by an iterative procedure. Also, an additional scaling is performed that takes into account columns of ( A – I ) that are fixed or have positive lower bounds or negative upper bounds. 



With the default setting ('Automatic') SNOPT uses 'Only scale linear rows and columns' for linear programs, and 'No scaling' otherwise.



If nonlinear constraints are present, the scales depend on the Jacobian at the first point that satisfies the linear constraints. Option 'Only scale linear rows and columns' should therefore be used only if a good starting point is provided and if the problem is not highly nonlinear.



Possible values are:



*	Automatic
*	No scaling
*	Only scale linear rows and columns
*	Additional scaling



