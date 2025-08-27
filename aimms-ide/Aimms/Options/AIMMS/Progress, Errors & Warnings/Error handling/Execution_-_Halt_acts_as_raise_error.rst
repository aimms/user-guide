

.. _option-AIMMS-halt_acts_as_raise_error:


Halt acts as raise error
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



The normal execution of a ``HALT``  statement does not respect any error handlers but will stop execution. If you would like ``HALT``  statement to be treated as an encountered error, you can do so by setting the this option on. Possible values of this option are:



    *	Off (Stop execution, regardless of any errors)
    *	On (Treat a ``HALT``  statement as if a ``RAISE ERROR``  is encountered)










**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`sec:exec.error`  



