.. _option-KNITRO-linear_system_form_used:


Linear System Form Used
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option indicates which linear system form is used inside the Interior/Direct algorithm for computing primal-dual steps. At the default value, Knitro automatically chooses the linear system form. Possible values are:



    *	Automatic
    *	Full linear system
    *	A compact system
    *	Most compact system
    *	Eliminate inequalities




Setting this option to 'Most compact system' may generate significant speedups on very large models. The 'Eliminate inequalities' setting may generate significant speedups on models where the number of variables is small, but the number of inequality constraints is large.

