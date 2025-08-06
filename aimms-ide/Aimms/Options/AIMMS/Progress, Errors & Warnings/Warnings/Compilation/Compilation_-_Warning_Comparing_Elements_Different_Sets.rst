

.. _Options_Compilation_-_Warning_Comparing_Elements_Different_Sets:


Warning Comparing Elements Different Sets
=========================================



Type:	Selection	

Range:	The settings listed below	

Default:	Warning_in_develop_else_off



When comparing two elements that have different range sets, the result may be different than you expect. 



Example:



Assume we have:


*   a set A with ordered content: { 'a', 'b', 'c', 'd' } 
*   a set B (subset of A) with ordered content: { 'd', 'a', 'c' }
*   an element parameter epAd in A with value 'd'
*   an element parameter epBa in B with value 'a'



What is then the result of the expression: epAd < epBa ? 



In set A, comparing 'd' < 'a' would result in 0, but the same expression in set B would result in 1.



The default behavior of AIMMS in this situation is that it will use the super set of the two sets (in this example, set A). In other words, it evaluates the expression as if it was specified as Ord(A,epAd) < Ord(A,epBd). If your intention is to compare the elements using set B, you should write the corresponding expression with the calls to function Ord explicitly.





With this option you can control whether you want to receive a warning or error on the described construct.



Possible values for this option are:




.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off




**Note** 

*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W`  
*	:ref:`Options_Warnings_-_Common_warning_default` 
*	:ref:`Options_Warnings_-_Strict_warning_default` 
*	:ref:`Options_Warnings_-_Communicate_warnings_to_end_users` 



