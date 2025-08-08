

.. _Navigation_Action_Update_an_Identifier:


Update an Identifier
====================

By default, all identifiers with a definition are updated automatically when they are displayed on a page. In some situations this behavior may not be favorable, for example if:

*	the execution of the definition takes a long time, and/or
*	executing the definition only makes sense after the user has entered multiple input values.

In that case you can add a statement to your model that removes the identifier from the pre-defined set CurrentAutoUpdatedDefinitions, and use the Update action of a button to manually update the definition.





To add an action to your object that updates an identifier:


1.	While in Edit Mode, open the Properties dialog box of the Object you wish to assign the action to.


2.	Change to the Action tab.


3.	Select the Update Identifier action from the Select Action to Add list.


The Update Identifier dialog box appears on the right hand side of the tab


4.	Type the name of the identifier you wish to update, or use the Identifier selection dialog box.


5.	Click Ok.





**Note** 

*	It makes no sense to enter the name of an identifier that does not have a definition, or that is part of the set CurrentAutoUpdatedDefinitions.




**Learn more about** 

*	:any:`CurrentAutoUpdatedDefinitions`






