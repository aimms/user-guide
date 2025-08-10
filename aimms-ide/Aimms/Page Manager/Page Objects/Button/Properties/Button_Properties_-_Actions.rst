

.. _Button_Button_Properties_-_Actions:


Button Actions
==================

**Description** 

A button can have one or a series of actions associated with it, which are run in the prescribed order when the button is clicked. The following actions are available.

*	Goto Page, this action opens another page using the page hierarchy that is defined in the Page Manager tree (or you can open the previously visited page).
*	Linked Page(s), this action opens one page or a series of pages. If you specify links to multiple pages, then there are extra options to indicate whether all, or only one (user) selected page should be opened.
*	Run, this action runs a procedure. 
*	Assignment, assigns a value or the value of an identifier to an identifier (this can be numeric, element, or string).
*	Update Identifier, this action updates an identifier by executing its definition.
*	Assertion Check, this action can perform a number of model assertions.
*	Menu Command, this action performs an AIMMS menu command.
*	Popup Menu, this action links a right mouse popup menu to the button
*	Close Page, this action closes the current page.
*	Help, this action opens the windows help file that is associated with the current project at a specified location.




**Note** 

*	If a run actions runs a procedure that returns the value –1, the subsequent actions in the button action list will not be executed.




**How to add an action that …** 

*	:ref:`Button_Action_Opening_Pages`  
*	:ref:`Button_Action_Running_a_Procedure`  
*	:ref:`Button_Action_-_Assigning_a_Value_to_` 
*	:ref:`Button_Action_Update_an_Identifier`  
*	:ref:`Button_Action_Performing_Assertion_Ch` 
*	:ref:`Button_Action_Performing_a_Menu_Comma` 
*	:ref:`Button_LinkingPopupMenu` 
*	:ref:`Button_Action_Opening_Help`  
*	:ref:`Button_Action_Closing_the_Current_Pag`  




**How to …** 

*	:ref:`Button_Action_Changing_the_Action_Ord` 






