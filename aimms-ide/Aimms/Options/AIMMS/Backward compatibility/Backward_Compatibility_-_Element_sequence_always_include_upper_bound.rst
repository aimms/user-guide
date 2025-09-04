

.. _option-AIMMS-element_sequence_always_include_upper_bound:


Element Sequence Always Include Upper Bound
===========================================



:Type:	Selection	
:Range:	One of the settings listed below	
:Default:	Off	



An element sequence can be specified using the syntax ``{ lo .. up by incr }``. Even if there is
no integer ``i`` such that ``up = lo + incr * i``, AIMMS might include ``up`` in the generated sequence,
depending on the configuration of this option.
For example, ``{ 1 .. 8 by 2 }`` generates the elements ``{ 1, 3, 5, 7 }`` when this option is switched
off and ``{ 1, 3, 5, 7, 8 }`` when this option is switched on.

Possible values are:

    *	On
    *	Off


**Learn more about** 

*	:ref:`option-AIMMS-warning_element_sequence_upperbound_not_included` 

