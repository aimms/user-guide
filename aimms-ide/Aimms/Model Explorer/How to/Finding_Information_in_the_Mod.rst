.. |img_def_Find_button_bmp| image:: images/Find_button.bmp
.. |img_def_Find_Again_button_bmp| image:: images/Find_Again_button.bmp


.. _Model-Explorer_Finding_Information_in_the_Mod:


Find Information in the Model Explorer
======================================

**Description** 

When your model grows, the number of cross-references between identifiers also grows. Although the Model Tree is expected to express a natural model structure, a single change to your model could affect several identifiers throughout the model. To find (and optionally replace) information in your model, AIMMS offers a text oriented find and replace mechanism (similar to the ones that are available in text editors) that is extended with some model specific features. 



To search for text only in some subset of identifier attributes, the Find dialog box is extended with a Model Specific tab. On this tab you can specify a subset of attributes that will be used to restrict the search process. When AIMMS finds the specified text in the attributes of some identifier it will open the corresponding identifier attribute form. 



To open the Find dialog box

1.	From the Edit menu, select Find… |img_def_Find_button_bmp|.



If you check the Entire Model checkbox, then AIMMS will search through all possible model text (both in the Model Tree itself and in all underlying attribute windows) and it will open a window automatically if the text is found. If you only want to search for text within the currently active window (either the Model Tree or an attribute window) then you should deselect the Entire Model checkbox.



If you are searching for text in the entire model, then AIMMS automatically opens a window in which it finds a match. To avoid that you end up with a lot of open windows during the search, you can select the Close Visited Window checkbox. If this option is selected, any window that is opened during the search will also be closed automatically when the search continues in another window.



If the search finds a match in any of the windows, the search will stop and the found text will be highlighted. If you want to continue searching for the next occurrence of the text:

1.	From the Edit menu, select Repeat Find |img_def_Find_Again_button_bmp|.



