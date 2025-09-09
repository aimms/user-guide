

.. _option-AIMMS-store_nonlinear_presolve_info:


Store Nonlinear Presolve Info
=============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option determines whether AIMMS will store MPI related information during the presolve of a nonlinear model.
Of course, this information is only available if you are solving a nonlinear model and :ref:`sec:nlp.presolve` has
been activated. Without this option set to 'Yes', the MPI will not report any information about the presolver. This
information includes information about bound reductions and eliminated rows and columns. Possible values are:

    *	No
    *	Yes


**Learn more about** 

*	:ref:`aimmshelp26-Math_Program_Inspector` 
*	:ref:`option-AIMMS-nonlinear_presolve` 

