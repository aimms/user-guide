

.. _option-AIMMS-transform_ellipsoids:


Transform Ellipsoids
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Both



To improve numerical stability for robust optimization problems with ellipsoidal uncertainty constraints (or regions), AIMMS can do two transformations before building the robust counterpart.



With setting 'Simplify' quadratic terms of the form (x - b)2, with x an uncertain parameter and b a normal parameter, will be transformed into y2 where y is an additional uncertain parameter satisfying y = x - b.



With setting 'Root' an uncertainty constraint of the form xTQx <= b will be transformed into sqrt( xTQx ) <= sqrt( b ). This transformation is valid if matrix Q is positive semi-definite.



At the default setting both transformations are applied. Possible values are:



*	Off
*	Simplify
*	Root
*	Both




**Note** 

*	Option **Boxed Ellipsoids**  can also be used to improve numerical stability.




**Learn more about** 

*	:ref:`option-AIMMS-boxed_ellipsoids`  



