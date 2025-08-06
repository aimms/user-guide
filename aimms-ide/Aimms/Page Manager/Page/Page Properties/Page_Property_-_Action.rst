

.. _Page-Manager_Page_Property_-_Action:


Action
======

**Description** 

On the Action Properties tab you can set the following properties:



**Page Entry Procedure** 

This option lets you specify a procedure that will be executed when the page is opened. The Page Entry Procedure should not have any arguments. Additionally, you can choose to update all identifiers that are contained in the page, when it is opened. Note that, by default, all identifiers with definitions are updated automatically when they are displayed on a page, and thus you do not need to update them explicitly. However, you can remove an identifier from the pre-defined set CurrentAutoUpdatedDefinitions, so that its definition is only updated when this is requested explicitly.



**Page Exit Procedure** 

The page exit procedure is executed when a page is about to be closed. If this procedure returns –1, the page will not be closed. For tabbed pages the exit procedure will be called when trying to switch to another page. If the procedure returns –1 you will not switch to the other page. If a page has a tabbed page object and the page is closed, first the active page in the tabbed page object will be closed, so also first the exit procedure of this active page will be called..



**Page Procedure** 

This option lets you specify a procedure that will be executed when a button is clicked for which the 'Run Page Procedure' property is checked. This is particular useful if a button is part of a template, so that you can still let (part of) the action depend on the page where the button is clicked. The Page Procedure should not have any arguments.



**System Menu Close** 

If you want to have control over when a user closes a page, then you should specify what to do if the user selects one of the system specific ways to close a window (i.e. pressing Ctrl-F4 (or Alt-F4 in case of a dialog box), or clicking on the [x] button in the top-right corner of the window). You can choose between:

*	Closing the window (default).
*	Ignore the close command.
*	Handle the close command as if an existing button on the page has been clicked. This button must be referenced using its tag name.
*	Execute a specified model procedure.

If you choose to close the page via a button reference or a procedure, then this button should have a close action or the procedure should make a call to PageClose.





**Note** 

*	When you decide to ignore page close commands and you have also specified the style Behave as Dialog for that page, you should make sure that there is at least one method to close the page (via buttons). If this is not the case, the end-user cannot close the dialog page at all. In developer mode you can always close a page with the [x] button, even when the system menu close is set to Ignore the close command. However in this situation a dialog will be displayed, warning the developer that an end-user might get stuck.
*	A template does not have a Property - Action tab.




**Learn more about** 

*	:ref:`Page-Manager_Tags`  
*	 Search for CurrentAutoUpdatedDefinitions (Function Reference)






