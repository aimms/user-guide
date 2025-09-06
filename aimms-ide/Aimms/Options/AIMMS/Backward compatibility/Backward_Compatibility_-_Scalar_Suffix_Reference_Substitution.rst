

.. _option-AIMMS-scalar_suffix_reference_substitution:


Scalar Suffix Reference Substitution
====================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



Possible values of this option are:

    *	On
    *	Off

Consider the following declarations:

.. code-block:: aimms

    Parameter x_lo {
        InitialData: 1;
    }
    Parameter x_up {
        InitialData: 5;
    }
    Parameter x_mid;
    Variable x_scalar {
        Range: [x_lo, x_up];
    }


With these declarations the result of the statement

.. code-block:: aimms

    x_mid := ( x_scalar.lower + x_scalar.upper ) / 2 ;

will depend on the setting of this option:

    *	When this option is off: 	 x_mid = 0
    *	When this option is on:	 x_mid = 3


**Learn more about** 

*	:ref:`option-AIMMS-warning_difference_scalar_suffix_reference_substitution` 

