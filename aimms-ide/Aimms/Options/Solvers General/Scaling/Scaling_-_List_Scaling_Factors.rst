

.. _option-AIMMS-list_scaling_factors:


List Scaling Factors
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	


This option controls whether AIMMS should print the scaling factors, found by one of its scaling algorithms,
to the listing file. Possible values are:

    *	Off
    *	Automatic
    *	Individual
    *	Symbolic


The scaling algorithm used by AIMMS is controlled by the option **Scaling Algorithm**. The Optimization based
algorithm scales variables and constraints at the symbolic level. This is illustrated by the following example:
if the model contains the variable ``X(i)``, with :math:`i` in {1,...,5}, then the scaling factor found for ``X(i)`` will be
the same for all :math:`i`, so the scaling factor found for ``X(1)`` will be the same as for ``X(2)`` to ``X(5)``. The other
two scaling algorithms, Iterative and Combination, find scaling factors at the individual (column and row) level.
Using the same example, the scaling factors found for ``X(i)`` might be different, so the scaling factor found for
``X(1)`` might be different than the one found for ``X(2)``.


The 'Symbolic' setting is only available if the **Scaling Algorithm** option has been set at 'Optimization Based',
or at 'Automatic' and (only) the Optimization Based algorithm is used. The 'Individual' setting is available for
all scaling algorithms, including the Optimization based algorithm.


At the 'Automatic' setting AIMMS will select 'Symbolic' if the **Scaling Algorithm** option has been set at
'Optimization Based', or at 'Automatic' and (only) the Optimization Based algorithm is used. AIMMS will select
'Individual' otherwise.


**Note** 

*	This option is only used if the option **Scale Model** has been switched on.
*	The scaling factors will also be printed in the listing file if the :ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model`  inside the Math Program Inspector is used and this option is set to 'Automatic' or 'Symbolic'.


**Learn more about** 

*	:ref:`option-AIMMS-scale_model` 
*	:ref:`option-AIMMS-scaling_algorithm` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Scale_Model` 

