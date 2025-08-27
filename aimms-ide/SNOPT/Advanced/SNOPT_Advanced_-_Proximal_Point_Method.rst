.. _option-SNOPT-proximal_point_method:


Proximal Point Method
=====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Euclidean	



This option specifies the expression that is minimized when the starting point x0 is changed to satisfy the linear constraints (where x0 refers to nonlinear variables).



Possible values are:



    *	Euclidean
    *	Quadratic




Euclidean means that ``|| x -`` x0``||``  will be minimized, while quadratic means that 0.5 ``|| x -`` x0``||`` 2 will be minimized.




