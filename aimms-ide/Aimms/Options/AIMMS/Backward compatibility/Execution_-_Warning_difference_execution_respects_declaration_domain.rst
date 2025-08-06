

.. _Options_Execution_-_Warning_difference_execution_respects_declaration_domain:


Warning Difference Execution Respects Declaration Domain
========================================================

**Type:** 	Selection	

**Range** :	The settings listed below	

**Default** :	Off	



When the option **Execution respects declaration domain**  in the Backward Compatibility category is set to On, this option specifies what happens when, during execution, there are differences with regard to the declaration domain (as specified by the option **Execution respects declaration domain** ). This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:



*	Off					- Do not issue a warning.
*	Warning_collect			- Issue a warning and post it to the global error and warning collector
*	Common_warning_default		- Take action depending on the option '``Common warning default`` '.
*	Warning_handle			- Issue a warning and post it to the nearest error handler
*	Strict_warning_default		- Take action depending on the option '``Strict warning default`` '.
*	Error				- Issue an error, and execution stops if the error limit specified by the option '``errors until halt`` ' is reached.




**Note** 

*	When there are differences in your model results, you may want to switch this option to Error or Warning in order to find the cause of those differences.
*	With the option **Maximal Number of Warnings Reported**  you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`Options_Warnings_-_Maximal_Number_of_W` 

*   :ref:`Options_Backward_Compatibility_-_Execution_respects_declaration_domain` 






