

.. _Navigation_Action_Closing_the_Current_Pag:


Closing the Current Page
========================

To add a button action that closes the current page:

1.	While in Edit Mode open the Properties dialog box of the Object you wish to assign the action to.

2.	Change to the Action tab.

3.	Select the Close Page action from the Select Action to Add list.

4.	Click Ok.



**Note** 

*	It is possible to check the 'abort further actions if not closed' flag. When a page is closed, first the page's Exit Page Procedure will be called. If the procedure returns the value –1, the page will not be closed. In this case, if you have set the 'abort further actions if not closed' flag, further actions in the action list will not be executed.



