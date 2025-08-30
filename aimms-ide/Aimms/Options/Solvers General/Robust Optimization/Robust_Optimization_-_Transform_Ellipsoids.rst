

.. _option-AIMMS-transform_ellipsoids:


Transform Ellipsoids
====================


:Type:	Selection	
:Range:	The settings listed below	
:Default:	Both


To improve numerical stability for robust optimization problems with ellipsoidal uncertainty constraints (or regions),
AIMMS can do two transformations before building the robust counterpart.


With setting 'Simplify' quadratic terms of the form :math:`(x - b)^2`, with :math:`x` an uncertain parameter and
:math:`b` a normal parameter, will be transformed into :math:`y^2` where :math:`y` is an additional uncertain
parameter satisfying :math:`y = x - b`.


With setting 'Root' an uncertainty constraint of the form :math:`x^TQx <= b` will be transformed into
:math:`\sqrt{x^TQx} \leq \sqrt{b}`. This transformation is valid if matrix :math:`Q` is positive semi-definite.


At the default setting both transformations are applied. Possible values are:

    *	Off
    *	Simplify
    *	Root
    *	Both


**Note** 

*	Option **Boxed Ellipsoids**  can also be used to improve numerical stability.


**Learn more about** 

*	:ref:`option-AIMMS-boxed_ellipsoids`  

