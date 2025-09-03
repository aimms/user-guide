

.. _option-AIMMS-adjustable_bound:


Adjustable Bound
================



:Type:	Floating point number	
:Range:	[0,inf)	
:Default:	inf	


For adjustable variables AIMMS automatically generates additional unbounded variables. For example,
if adjustable variable ``x(i)`` depends on an uncertain parameter ``a(j)`` then AIMMS will generate variables
``x.Adjustable.a(i,j)`` and ``x.Adjustable.Constant(i)``. By default these variables have a lower bound of
-inf and an upper bound of inf. In case the robust counterpart is a second-order cone program (SOCP),
the solver might sometimes face difficulties solving it. In that case it sometimes helps the solver to
add finite bounds for the .Adjustable variables.

If an adjustable variable has no upper bound then the upper bound used will be equal to the value of
this option. If an adjustable variable has no lower bound then the lower bound used will be equal
to the value of this option multiplied by -1.

You can also assign lower and upper bounds to .Adjustable variables without using this option. For
example, you can use in your model the following statements:


.. code-block:: aimms

    x.Adjustable.a.upper(i,j) := 1000;
    x.Adjustable.a.lower(i,j) := -1000;

