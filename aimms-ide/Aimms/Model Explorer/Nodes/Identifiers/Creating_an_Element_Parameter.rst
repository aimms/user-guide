.. |img_def_Identifier_Element_Parameter_bmp| image:: images/Identifier_Element_Parameter.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_an_Element_Parameter:


Creating an Element Parameter
=============================

**Description** 

To create a new element parameter in the Model Tree:

1.	Select the position in a Declaration Section where the new element parameter should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Element_Parameter_bmp| Element parameter and press OK

4.	Enter a name for the new element parameter (if you are creating a multi-dimensional parameter, you can type the indices of each dimension as well)

5.	Press ``<Enter>``  to create the new element parameter (or press ``<Esc>``  to abort the operation)



The newly created element parameter is not yet ready for use, because you still have to specify the range set via its attributes. To modify the attributes of the newly created element parameter:

*	Press ``<Enter>``  or double click on the element parameter.




The most commonly used attributes of an element parameter are discussed below. 




*	``INDEX DOMAIN``: The ``INDEX DOMAIN`` attribute should be specified in order to declare indexed element parameters. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``RANGE``: The ``RANGE`` attribute should be used to specify the set in which the element parameter should take its value. The |img_def_Wizard_button_bmp| wizard will display an Identifier Selection Dialog box that helps you select the appropriate set.
*	``DEFAULT``: The ``DEFAULT`` attribute should be used in order to specify a default value other than the empty element. Note that AIMMS will explicitly store all values that are non-default. 
*	``DEFINITION``: The ``DEFINITION`` attribute can (and should) be used to specify the definition of an identifier by means of a global relationship. AIMMS stores the result of a definition and recomputes it only when necessary.




**Remark** 


A common way to declare a scalar element parameter is on the attribute form of the associated set identifier.





**How to ...** 

*	:ref:`Model-Explorer_Creating_a_Set`  




**Learn more about** 

*	:ref:`element_parameter`
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:doc:`non-procedural-language-components/execution-of-nonprocedural-components/dependency-structure-of-definitions`
*	:ref:`Miscellaneous_Identifier_Selection_Dialog_Bo` 

.. *	:doc:`AIMMS Update Mechanism <>`


