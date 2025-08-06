

.. _Shared-Object-Properties_Object_Properties_-_Element_Te:


Element Text
============

**Description** 

In the Element Text tab of an object property dialog box, you can specify alternative text for set element names that are visible in the object. This property tab shows a list of all indices (or sets) that are used in the object, and for each entry in this list you can specify a text that will replace the corresponding element names.

For example, if you have a table for identifier A(i), then you can replace the displayed names of the element in i via:

*	a one-dimensional string parameter MyNames(i), so that an element 'i01' is replaced by the value MyNames('i01'),
*	a scalar string parameter, or
*	a static string.

Of course, for the latter two, all elements will be replaced by the same text.





**Tips & Tricks** 

*	By using string parameters that replace the element names, you can display alternative element text for different languages.
*	If you explicitly specify the empty string "", you choose not to display any text for a specific index.



