

.. _Navigation_Navigation_Object_Properties_1:


Navigation Actions
===================

**Description** 

The standard action of a Navigation object is the opening of the selected page. 
In addition to this you can specify other actions that should be performed before or after the page open action. You can specify these additional actions in a similar way as for the button object. The following actions are available:

*	Open selected navigation page, this is the standard navigation action, and cannot be remove from the list.
*	Run, this action runs a procedure. 
*	Assignment, assigns a value or the value of an identifier to an identifier (this can be numeric, element, or string).
*	Update Identifier, this action updates an identifier by executing its definition.
*	Assertion Check, this action can perform a number of model assertions.
*	Menu Command, this action performs an AIMMS menu command.
*	Close Page, this action closes the current page.
*	Help, this action opens the windows help file that is associated with the current project at a specified location.




**How to add an action that …** 

*	:ref:`Navigation_Action_Running_a_Procedure`  
*	:ref:`Navigation_Action_-_Assigning_a_Value_to_`  
*	:ref:`Navigation_Action_Update_an_Identifier`  
*	:ref:`Navigation_Action_Performing_Assertion_Ch` 
*	:ref:`Navigation_Action_Performing_a_Menu_Comma` 
*	:ref:`Navigation_Action_Closing_the_Current_Pag`  
*	:ref:`Navigation_Action_Opening_Help`  




**Note** 

*	If a run actions runs a procedure that returns the value –1, the subsequent actions in the navigation object action list will not be executed.




**How to …** 

*	:ref:`Navigation_Action_Changing_the_Action_Ord`  



