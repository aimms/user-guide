

.. _Scalar_Scalar_Object_Properties_-_Sca:


Scalar
======

**Description** 

On the Scalar tab of the properties dialog box, you can modify the general appearance of the scalar object.



**Display** 

There are five display styles that determine whether (and where) a descriptive text is shown, and whether an edit field is always visible (or only appears when starting to edit a value). These styles are:

*	Value(s) only. (Only the value is shown, edit field only appears when needed)
*	Text – Value. (A descriptive text is shown at the left side, edit field only appears when needed)
*	Value – Text. (A descriptive text is shown at the right side, edit field only appears when needed)
*	Single Line Edit Field. (Only the value is shown, a single line edit field is always available)
*	Multiple Line Edit Field. (Only the value is show, a multiple line edit field is always available).

If you select the Multiple Line Edit Field (which is only available for string parameters), you can also choose to have scrollbars within the object. If you do not choose to display a horizontal scrollbar, then the text will not exceed the right boundary of the object and is automatically 'wrapped' to the next line.





**Password Style** 


This option is only available for the Single Line Edit Field. With this option you can create an input field for a scalar string parameter that behaves like a password input: instead of showing the entered text each character is displayed by a * sign. Besides that, the Copy and Cut features are disabled. Please note that inside the Aimms model, the string is stored exactly as it is typed, so you should be careful that the string cannot be made visible somewhere else in the GUI. Perhaps it is best to clear the string parameter after it is accepted.





**Display Referred Text File** 


This option is only available for the Multiple Line Edit Field. If you select this option, then the scalar object will not display the value of the string parameter, but instead regards this value as a file name and (if the file exists) the object will display the contents of this file. This file should be a text file and it is shown as read-only.





**Separator Sign** 


If you have selected either of the two display styles Text-Values or Values-Text, then you can choose which character should be placed between the text and the descriptive text. If you do not want to display a separator character you can leave the field empty.





**Show Inactive Data** 


If this option is not selected, inactive data will be considered to have a default value. In the scalar object this means that if you explicitly display an inactive element then the default value is shown. You can read more about inactive data in the Language Reference.





**Multiple Case Object** 


If you choose the multiple case object option, the data from different cases will be shown in different columns in the scalar object. You can add an extra column to the scalar object that contains the sum of all columns or the value in the first minus the value in the second column or the value in the second minus the value in the first column. You can set the number of visible columns. If the number of columns is less than the number of cases for which data is displayed the scalar object will be equipped with a horizontal scrollbar. It is possible to display the case name above each column.





**Note** 

*	If you want the Enter key to work as a end-of-line you should make sure that on the Misc tab of the Scalar object the Leave Object on Enter switch is turned off.




**Learn more about** 

*	 :ref:`inactive_data`
*	:ref:`Scalar_Object_Properties_-_Miscellane`  



