.. |uum| unicode:: U+00FC .. uum

.. _option-AIMMS-reformulate_constraints:


Reformulate Constraints
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Multi	



This option controls whether the AIMMS Presolver should try to reformulate constraints during MINLP probing. Possible values are:

    *	Off
    *	Single
    *	Multi


The AIMMS Presolver can transform some classes of nonlinear constraints into equivalent linear constraints.
For example, under some conditions it is possible to transform a constraint of the form

.. math::

    a * x + b * x * y + c * y \leq d


where :math:`x` is a binary variable and :math:`y` a continuous or integer variable, into a linear constraint.
Furthermore, for a set of constraints of the form

.. math::

    y \leq x \\
    y^2 \leq z


where :math:`x` is a binary variable and :math:`y` and :math:`z` are continuous variables, the second constraint
can be transformed into its perspective counterpart resulting in a tighter relaxation. See G\ |uum|\ nl\ |uum|\ k et al. (2010).

With setting 'Single' the AIMMS Presolver will only transform constraints if their counterpart consists of one
constraint. With setting 'Multi' also constraints are transformed for which the counterpart requires more than
one constraint. For inequalities the AIMMS presolver can add one additional constraint and for equalities up
to three additional constraints. The suffix .ExtendedConstraint can be used to refer to these additional
constraints. For example, the first additional constraint for constraint c(i) is labeled as
c(i).ExtendedConstraint('Linearization'), the second as c(i).ExtendedConstraint('Linearization2'), and so on.

Setting 'Multi' is only applied if the GMP function :any:`GMP::Instance::CreatePresolved` is used! If a normal
solve statement is used then the 'Multi' setting is equivalent to the 'Single' setting.


**Note** 

*	This option has only an effect if the option **MINLP Probing** is switched on.
*	For some MINLP problems it might be worthwhile to experiment with the function :any:`GMP::Instance::CreatePresolved` if you are using BARON or Knitro. (The GMP-AOA algorithm already uses the function :any:`GMP::Instance::CreatePresolved` underneath.)


**Learn more about** 

*	:ref:`option-AIMMS-minlp_probing` 


**References** 

*	G\ |uum|\ nl\ |uum|\ k, O., and J. Linderoth, Perspective reformulations of mixed integer nonlinear programs with indicator variables, Math. Program. B **124** (2010), pp. 183-205.



