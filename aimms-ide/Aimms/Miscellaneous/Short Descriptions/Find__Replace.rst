.. |img_def_Find_button_bmp| image:: images/Find_button.bmp
.. |img_def_Find_Again_button_bmp| image:: images/Find_Again_button.bmp


.. _Miscellaneous_Find__Replace:


Find & Replace
==============

**Description** 

The Find & Replace dialog box in AIMMS has a Find tab, and a Model Specific tab, which is only available when you are using the find and replace in the Model Explorer or the Attribute windows.



On the Find tab, you can specify the standard find and replace options, such as the text to find and the optional replacement text, the direction of the search, whether the comparison should be case-sensitive, and whether only whole words should be searched. 



To help you in finding the declaration of s specific model identifier, you can click on the Declaration button. This button is enabled only if the current search text represents a valid identifier in your model. When you click on this button, the dialog box closes, and AIMMS highlights the position of the specific identifier declaration in the Model Explorer. The functionality of this Declaration button is also available in the :ref:`Miscellaneous_Identifier_Info`  dialog box.



On the Model Specific tab, you can specify additional options to search only in specific parts of your model. It allows you to only search in a specified subset of attributes, or to search only in the currently active window and not in the entire model. If you search in the entire model, then AIMMS will automatically open the attribute windows in which the specified text is found. On the Model Specific tab you can also specify whether these opened windows are automatically close when you continue the search.



You can initiate a find (and replace) action by selecting |img_def_Find_button_bmp| Find from the Edit menu. To repeat the last find (and replace) you can select |img_def_Find_Again_button_bmp| Repeat Find from the Edit menu.





