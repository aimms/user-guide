

.. _option-AIMMS-warning_incompatible_binding_in:


Warning Incompatible Binding IN
===============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Warning_in_develop_else_off	



This option controls a warning on a binding IN for which the handling has changed since AIMMS version 25.1.



This situation is ignored, reported as a warning, or interpreted as an error, depending on the following settings:




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




An example of such a situation arises in the definition of pcard in the following model fragment:



``SET A {`` 

``Index i;`` 

``InitialData: data { i1 .. i2 }`` 

``}`` 

``SET RootSet {`` 

``InitialData: data { 1 .. 10 };`` 

``SET MySubSet {`` 

``Index: sm;`` 

``:Range: RootSet;`` 

``InitialData: data { 3, 4 };`` 

``}`` 

``SET MyIndexedSet {`` 

``Index: i;`` 

``:Range: RootSet;`` 

``InitialData: data { i1 : { 1, 3, 5 }, i2 : { 6, 7 } };`` 

``}`` 

``PARAMETER pcard {`` 

``Index: i;`` 

``Definition: count( sm IN MyIndexedSet(i) );`` 

``}`` 



In AIMMS versions before 25.1 this would result in pcard having the following data: { i1 : 1, i2 : 0 }, while it should have been { i1 : 3, i2 : 2 }

This is because in the older versions the definition of pcard, was executed as it it was specified as: count( sm IN MyIndexedSet(i) **| sm IN MySubset**  )



If you intend to use it the 'old' way then you must now specify the extra binding IN explicitly.



**Note** 

*	With the option Maximal Number of Warnings Reported you can set the maximal number of warnings that are shown in errors/warnings and message window.




**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 






