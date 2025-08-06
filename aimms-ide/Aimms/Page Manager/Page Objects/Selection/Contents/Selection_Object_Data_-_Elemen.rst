.. |img_def_radiobuttons_bmp| image:: images/radiobuttons.bmp


.. _Selection_Selection_Object_Data_-_Elemen:


Selection Object Data - Element Parameter
=========================================



**Description** 

An element parameter is the most natural way to store a single selected element from a list of set elements. It can, of course, only be used in combination with single selection controls (radio buttons, drop-down list, or list box).



When using an element parameter, the list of options from which the user can select corresponds to the range set of the parameter.



**Example** 

Data:

	``Cities := data { 'Amsterdam', 'Rotterdam', 'The Hague' };`` 

	``SelectedCity := 'Rotterdam' ;`` 

Corresponding radio buttons:



|img_def_radiobuttons_bmp|



