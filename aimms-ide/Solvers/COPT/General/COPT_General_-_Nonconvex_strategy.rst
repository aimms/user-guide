.. _option-COPT-nonconvex_strategy:


Nonconvex Strategy
==================



:Type:	Selection
:Range:	The settings listed below
:Default:	Automatic



This option determines the strategy for handling continuous nonconvex models, i.e., QP and QCP models for which the objective or a quadratic constraint is
nonconvex (including models with quadratic equality constraints). Possible values are:

    *	Automatic
    *	Off
    *	Local optimal solution
    *	Global optimal solution


With setting 'Off', COPT reports that the model is nonconvex and terminates. With setting 'Local optimal solution', COPT searches for a local optimum;
with setting 'Global optimal solution', COPT searches for a global optimum using branch-and-bound. With setting 'Automatic', COPT decides; for nonconvex
QP models it typically searches for a local optimum.

This option only applies to continuous models. Nonconvex MIQP and MIQCP models are always solved to global optimality, even if this option is set to 'Off'.


**Note**

*	This option was added in COPT 8.0.
