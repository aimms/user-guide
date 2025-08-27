

.. _option-AIMMS-ignore_variable_inline_property:


Ignore Variable Inline Property
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



When this option is set the inline property of variables is ignored. This option is only applicable compile time; changing this option should be followed by F5 (entire model compilation). 



Some solvers benefit from inlined variables while others do not. Changing from one solver to the next we can set this option to test whether or not inlining variables is beneficial for the current combination of application and solver.



Possible values are:



    *	On
    *	Off






