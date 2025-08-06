

.. _Navigation_Action_Running_a_Procedure:


Running a Procedure
===================

To add an action to your object that runs a model procedure:

1.	While in Edit Mode, open the Properties dialog box of the Object you wish to assign the action to.

2.	Change to the Action tab.

3.	Select the Run action from the Select Action to Add list.

The Run dialog box appears on the right hand side of the tab

4.	If you want to run the page procedure select Page Procedure, else select Procedure.

5.	Type the name of the procedure you want to run, or use the Identifier selection dialog box.

6.	You can also specify a procedure with element-valued arguments, in which case you have to specify elements or element parameters for all arguments.

7.	If you want the procedure to run in the background, check Run in Background.

8.	If you want to abort the sequence of actions if errors occur during the run, check Abort further Actions on Error.

9.	Click Ok.



**Note** 

*	By default, AIMMS does not run a procedure in background. This means that you have to wait for the procedure to finish before continuing. If you choose a to run a procedure in background, you do not have to wait for the procedure to finish, and in the meantime you can browse through your data and switch to other pages. You should be careful when using this option, because browsing through the data and opening pages may involve the execution of other procedures and changes in the values of element parameters, and this could influence the execution of the procedure that is running in background.
*	The Page Procedure is specified in the property dialog box of a page. Running the Page Procedure is especially useful if the button is created on a template. You can then use the template mechanism to define a button that has a standard look and feel for every page, but its action is specific for the page on which it is displayed. For example you can create standard template buttons for navigating to the next or previous page, but before doing so you can run a procedure that checks the data that is specific for the current page.




**Remark** 


When you have activated the Abort further Actions on Error option, the following situations will be recognized as error:

*	AIMMS execution errors.
*	Failed assertions.
*	Abort statements.
*	A return value of -1 from the procedure.

This last option makes it possible for the user to decide whether or not button actions should be performed depending on model data.







