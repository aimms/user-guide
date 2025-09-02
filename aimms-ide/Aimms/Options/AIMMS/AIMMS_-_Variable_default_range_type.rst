

.. _option-AIMMS-variable_default_range_type:


Variable default range type
===========================



:Type:	Selection
:Range:	The settings listed below	
:Default:	Free	



When a variable is created in the model editor, the range attribute of that variable is immediate filled in. With this option,
this default fill in can be controlled. Depending on the value of this option, one of the following four words is filled in by default:


    *	Binary {0, 1}
    *	Free (-inf, inf)
    *	Integer {0 .. :ref:`Miscellaneous_Maxint`}
    *	Nonnegative [0, inf)


**Learn more about** 

*	:ref:`sec:var.var` 
