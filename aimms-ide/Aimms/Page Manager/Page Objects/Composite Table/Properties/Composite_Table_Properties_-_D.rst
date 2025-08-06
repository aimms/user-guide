

.. _Composite-Table_Composite_Table_Properties_-_D:


Domain
======

**Description** 

On the Domain tab of the Composite Table properties dialog box, you can set options concerning the current row selection and the allowed modifications to the row domain (adding, removing and modifying rows).

Note: all the properties on this tab are ignored if you have disabled the option Row Selection on the Table tab.



**Store Selection in:** 

Via the identifier that you fill in here, you can keep track of the current row selection in the Composite Table or change the current row selection from within your model. The identifier should have an index domain that matches the domain identifier of the Composite Table. The values of the identifier are interpreted (and set) as follows: a value of 1 (or any value not equal to 0) corresponds to a selected row, a value of 0 corresponds to a deselected row.



**Allowed Actions** 

With the options below you define whether or not the user is allowed to make specific changes to the domain of the Composite Table. If the domain identifier is an Index, then the actions correspond to adding, removing or renaming the elements of a set. If the domain identifier is an indexed parameter, then the actions correspond to setting the values of the identifier to or from their default value.



**Add Row** 

If you select this option, the end-user will be able to add rows to the Composite Table (using the Insert key). Adding rows means that the domain identifier is modified:

*	If the domain is an index, adding a row corresponds to adding an element to the set.
*	If the domain is an indexed identifier, adding a row implies that an element of the identifier is set to a value other than the default value.




**Delete Row(s)** 


If you select this option, the end-user will be able to remove rows from the Composite Table (using the Delete key). Deleting rows means that the domain identifier is modified:

*	If the domain is an index, deleting a row corresponds to removing an element from the set.
*	If the domain is an indexed identifier, deleting a row implies that the corresponding element in the identifier data is set to its default value.




**Modify Rows** 


If you select this option, the end-user will be able to modify rows from the Composite Table (using the F2 key). Modifying rows means that the domain identifier is modified:

*	If the domain is an index, modifying a row corresponds to renaming the corresponding set element.
*	If the domain is an indexed identifier, modifying a row implies that the current element (tuple) is set to its default value, and the newly specified element (tuple) is set to a value other than the default value.




If your model needs to keep track of which elements are added, deleted, or modified, then you can specify your own procedures for each of these actions. These procedures will be called after the changes have taken place. In combination with the identifier in which the current selection is stored, you can check inside these procedures which elements (or tuples) are involved.





**Learn more about** 

*	:ref:`Composite-Table_Adding_Modifying_and_Removing_`  



