

.. _Table_Object_Properties_-_Assert:


Assert
======

**Description** 

On the Assert tab of the object properties dialog box, you can specify which assertions should be verified after the user makes a change to the data in the object. For every identifier contained in the object you can specify a list of assertions to be checked.

If any of the assertions fails and the assertion does not have an associated action, a dialog box appears in which the assertion message is displayed. In this dialog box, the user can choose to either undo the data change or (if it is only a warning) ignore it. If the assertion has an associated action, then this action is executed upon failure and no dialog box is displayed (unless the action itself shows a dialog box).

Any of the assertions in the list can be marked as a Delayed assertion. This means that the assertion check on the changed data is only executed when this is explicitly given as a button action.



You need delayed assertion checks, if the assertion can only be verified after multiple data changes have been made by the user. For example, if a table contains a list of percentages that should all add-up to 100%, then it makes no sense to verify the assertion after each individual data change, because the user should at least be able to change two values. In this situation you choose to verify the delayed assertion when the user presses a button that closes the page.



**Learn more about** 

*	:ref:`Model-Explorer_Assertions` 
*	:ref:`Button_Button_Properties_-_Actions` 



