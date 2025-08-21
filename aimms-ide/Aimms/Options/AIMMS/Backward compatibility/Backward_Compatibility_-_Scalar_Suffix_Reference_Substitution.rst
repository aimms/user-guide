

.. _option-AIMMS-scalar_suffix_reference_substitution:


Scalar Suffix Reference Substitution
====================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	On	



Consider the following declarations:



  PARAMETER:

    identifier  : x_lo 

    initial data : 1 ;



  PARAMETER:

    identifier  : x_up 

    initial data : 5 ;



  PARAMETER:

    identifier  : x_mid ;



  VARIABLE:

    identifier  : x_scalar

    range    : [x_lo, x_up] ;



With these declarations the result of the statement:



    x_mid := ( x_scalar.lower + x_scalar.upper ) / 2 ;



Will depend on the setting of this option:



   When this option is off: 	 x_mid = 0

   When this option is on:	 x_mid = 3



Possible values of this option are:



*	Off
*	On




**Learn more about** 

*	:ref:`option-AIMMS-warning_difference_scalar_suffix_reference_substitution` 



