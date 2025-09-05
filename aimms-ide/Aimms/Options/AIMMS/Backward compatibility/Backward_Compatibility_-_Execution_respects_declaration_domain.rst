

.. _option-AIMMS-execution_respects_declaration_domain:


Execution Respects Declaration Domain
=====================================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	On	



This option determines whether AIMMS should respect the declaration domain during execution.
For example:

.. code-block:: aimms

    Set S {
        Index: i;
    }
    Set T {
        SubsetOf: S;
        Index: j;
    }
    Parameter P {
        Index: j;
    }

The statement ``A := sum( i, P(i) )`` should only consider the elements in ``S`` that also exist in ``T``.
This is the case when this option is set to 'On'. When you want to use the old behavior (all elements
in ``S`` are considered), you should switch this option to 'Off'. Possible values are:

    *	On
    *	Off


**Note** 

*	When there are differences in your model results, you may want to switch the option **Warning Difference Execution Respects Declaration Domain** to 'Error' or 'Warning' in order to find the cause of those differences.


**Learn more about** 

*	:ref:`option-AIMMS-warning_difference_execution_respects_declaration_domain`  

