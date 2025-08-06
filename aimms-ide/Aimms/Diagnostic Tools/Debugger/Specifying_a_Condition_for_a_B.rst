

.. _Diagnostic-Tools_Specifying_a_Condition_for_a_B:


Specifying a Condition for a Breakpoint
=======================================

To specify the condition on an existing breakpoint, you must open the Breakpoint Condition dialog. You can do this either from within the List of Breakpoints dialog box:

1.	Open the List of Breakpoints dialog box.

2.	Select the breakpoint for which you want to specify the condition.

3.	Push the Condition button.

Or via the right mouse popup menu of an existing breakpoint:

1.	Click the right mouse button on the breakpoint icon in the yellow margin of the attribute window.

2.	From the popup menu, select Breakpoint Condition. 



In the Breakpoint Condition dialog you can specify a simple scalar condition based on the comparison of numerical, element or string values.



**Note** 

*	AIMMS will only stop at a conditional breakpoint, when the condition that you have specified is met during a particular call. 
*	Conditional breakpoints are very convenient when, for instance, a procedure is called very frequently, but only appears to contain an error in one particular situation, which can be detected through a simple comparison.




**How to ...** 

*	:ref:`Diagnostic-Tools_Setting_a_Breakpoint`  
*	:ref:`Diagnostic-Tools_Stepping_through_the_Execution` 







**Learn more about** 

*	:ref:`Diagnostic-Tools_List_of_Breakpoints_Dialog_Box`  






