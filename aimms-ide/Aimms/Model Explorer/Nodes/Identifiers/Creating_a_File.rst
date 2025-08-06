.. |img_def_Identifier_File_bmp| image:: images/Identifier_File.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_File:


Creating a File
===============

**Description** 

To create a new file identifier in the Model Tree:

1.	Select the position in a Declaration Section where the new file identifier should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_File_bmp| File and press OK

4.	Enter a name for the new file identifier

5.	Press ``<Enter>``  to create the new file (or press ``<Esc>``  to abort the operation)



The newly created file identifier is now ready for use, but you probably want to specify some additional attributes. To modify the attributes of the newly created file identifier:

*	Press ``<Enter>``  or double click on the file node.




The most commonly used attributes of a file identifier are discussed below. 




*	``NAME``  : The ``NAME``  attribute is used to specify a name by which the file can be reference within AIMMS. The |img_def_Wizard_button_bmp| wizard will display a menu allowing you to specify either a system filename or a string parameter from your model that will be used to specify the filename.
*	``DEVICE``  : The ``DEVICE``  attribute should contain one of ``disk`` , ``window``  or ``void`` . The |img_def_Wizard_button_bmp| wizard will let you specify the ``DEVICE`` attribute through a selection of radio buttons.
*	``MODE``  : The ``MODE``  attribute should contain one of ``replace``  or ``merge`` . The |img_def_Wizard_button_bmp| wizard will let you specify the ``MODE`` attribute through a selection of radio buttons.




**Learn more about** 

*	Search for File identifiers and file attributes (Language Reference)
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation` 



