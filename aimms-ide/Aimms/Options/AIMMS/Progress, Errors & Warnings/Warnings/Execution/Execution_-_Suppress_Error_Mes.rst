

.. _Options_Execution_-_Suppress_Error_Mes:


Suppress Error Messages of Val Function
=======================================



Type:	Selection	

Range:	The settings listed below	

Default:	Off	



The function ``val``  translates strings to numbers. For example, ``val("2009")``  yields the number 2009. For strings that do not have an associated numerical value, ``val``  results into UNDF, for example, ``val("hello")=UNDF`` . For the default setting of this option ("Off"), the latter use of ``val``  results in an error message. However, in some situations it can be useful to continue after such an occurrence. Possible values of this option are:



*	Off (do not suppress error messages of the function val)
*	On (suppress error messages of the function val)




**Note** 

*	The section of the reference manual: "Raising and handling warnings and errors" provides a more powerful and transparent method for error handling.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 
*	:ref:`sec:exec.error`  



