.. |img_def_Debugger_step_bmp| image:: images/Debugger_step.bmp
.. |img_def_Debugger_step_into_bmp| image:: images/Debugger_step_into.bmp
.. |img_def_Debugger_step_out_bmp| image:: images/Debugger_step_out.bmp
.. |img_def_Debugger_run_to_current_bmp| image:: images/Debugger_run_to_current.bmp
.. |img_def_debugger_go_bmp| image:: images/debugger_go.bmp
.. |img_def_debugger_finish_bmp| image:: images/debugger_finish.bmp
.. |img_def_Debugger_halt_execution_bmp| image:: images/Debugger_halt_execution.bmp
.. |img_def_Debugger_show_current_statement_bmp| image:: images/Debugger_show_current_statement.bmp
.. |img_def_Debugger_show_call_stack_bmp| image:: images/Debugger_show_call_stack.bmp


.. _Diagnostic-Tools_Stepping_through_the_Execution:


Stepping through the Execution of a Model using Breakpoints
===========================================================

**Description** 

Once you have placed one or more breakpoints in your mode, AIMMS will automatically stop at these breakpoints whenever a line of execution arrives at the corresponding statement. 

Whenever the execution stops at a breakpoint, AIMMS will open the corresponding attribute window, and show the current line of execution through the breakpoint pointer, an open right arrow.



Once you have interrupted the execution, AIMMS offers several methods to step through the code:

*	The Step Over |img_def_Debugger_step_bmp| method runs a single statement, and, when this statement involves a function or a procedure call, executes this in its entirety unless other breakpoints are encountered.
*	The Step Into |img_def_Debugger_step_into_bmp| method runs a single statement, but, when this statement involves a function or procedure call, it will step into this function or procedure and set the breakpoint pointer at the first statement in this function or procedure.
*	The Step Out |img_def_Debugger_step_out_bmp| method runs to the end of the current function or procedure and sets the breakpoint pointer to the statement directly following the procedure call in the calling context, unless other breakpoints are encountered.
*	The Run to Cursor |img_def_Debugger_run_to_current_bmp| method runs in a single step from the current position of the breakpoint pointer to the current location of the cursor, which should be position somewhere in the body text of a function or procedure. If any other breakpoint is encountered before reaching the statement that is indicated by the cursor, the execution stops at that breakpoint.




In addition AIMMS offers some methods to continue or halt the execution:

*	The Continue Execution |img_def_debugger_go_bmp| method continues execution, but will stop at any breakpoint it will encounter during execution.
*	The Finish Execution |img_def_debugger_finish_bmp| method finishes the current execution sequence, ignoring any further breakpoints it encounters.
*	The Halt |img_def_Debugger_halt_execution_bmp| method immediately halts the current execution. Similar as the HALT statement, it directly jumps out of all procedures in the current call stack.




As well as some methods to determine where in the model the execution is currently interrupted:

*	The Show Current Position |img_def_Debugger_show_current_statement_bmp| command returns the cursor and the focus to the interrupted statement, and
*	The Call Stack |img_def_Debugger_show_call_stack_bmp| command opens the Call Stack dialog box with a detailed overview of the stack of procedure calls associated with the current line of execution.




**Note** 

*	Even when you have not set breakpoints, you can still enter the debugger by explicitly interrupting the current line of execution through the Run – Stop menu and pushing the Debug button.




**Learn more about** 

*	:ref:`Diagnostic-Tools_Call_Stack_Dialog_Box`  






