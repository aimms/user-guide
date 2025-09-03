

.. _option-AIMMS-warning_index_of_set_also_in_definition:


Warning Index of Set also in Definition
=======================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default	



When an index is declared in the set, and also used in the definition of that same set,the result may be unexpected. This option controls whether to ignore such a situation, warn about it, or even raise an error:






.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector.
   * - *	Common_warning_default
     - Take action depending on the option 'Common warning default'.
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler.
   * - *	Strict_warning_default
     - Take action depending on the option 'Strict warning default'.
   * - *	Error
     - Issue an error.
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off




Consider the following example:



SET:

 identifier : ExampleRootSet

 index   : ers

 definition : Data{R1..R10} ;



SET:

 identifier : ExampleSubset

 subset of : ExampleRootSet

 index   : ess

 definition : {ess | 1} ;



In the above example, the index ess is both declared as an index of ExampleSubSet, and it is used in the definition. The result of this definition, is empty however. In contrast, when using the definition { ers | 1 } all elements will be added to the set ExampleSubset.



**Note** 

*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 






