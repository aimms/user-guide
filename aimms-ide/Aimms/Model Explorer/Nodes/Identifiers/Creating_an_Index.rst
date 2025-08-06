.. |img_def_Identifier_Index_bmp| image:: images/Identifier_Index.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_an_Index:


Creating an Index
=================

**Description** 

The most common way to creating indices in a set is via the ``INDEX``  attribute of a set, but in some situations you should create the index as a node in the model tree (for example when you create a 'free' index, or an index in a pre-declared set).



To create a new index in the Model Tree:

1.	Select the position in a Declaration Section where the new index should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Index_bmp| Index and press OK

4.	Enter a name for the new index

5.	Press ``<Enter>``  to create the new index (or press ``<Esc>``  to abort the operation)



The newly created index is ready for use (as a 'free' index), but you probably want to specify the range of the index via its attributes To modify the attributes of the newly created index:

*	Press ``<Enter>``  or double click on the index.




The most commonly used attribute of an index is discussed below.




*	``RANGE``  : The ``RANGE``  attribute should be used to specify the set in which the index should take its value. If not specified, the index has no default binding to a specific set and can only be used in the context of local or implicit index binding. The |img_def_Wizard_button_bmp| wizard will display an Identifier Selection Dialog box that helps you select the appropriate set.




**How to ...** 

*	:ref:`Model-Explorer_Creating_a_Set`  




**Learn more about** 

*	Search for Indices and index attributes (Language Reference)
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`Miscellaneous_Identifier_Selection_Dialog_Bo`  



