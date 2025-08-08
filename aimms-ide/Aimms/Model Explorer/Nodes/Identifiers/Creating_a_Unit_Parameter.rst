.. |img_def_Identifier_Unit_Parameter_bmp| image:: images/Identifier_Unit_Parameter.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Unit_Parameter:


Creating a Unit Parameter
=========================

**Description** 

To create a new unit parameter in the Model Tree:

1.	Select the position in a Declaration Section where the new unit parameter should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Unit_Parameter_bmp| Unit parameter and press OK

4.	Enter a name for the new unit parameter (if you are creating a multi-dimensional parameter, you can type the indices of each dimension as well)

5.	Press ``<Enter>``  to create the new unit parameter (or press ``<Esc>``  to abort the operation)



The newly created unit parameter is now ready for use, but you probably want to specify some additional attributes. To modify the attributes of the newly created unit parameter:

*	Press ``<Enter>``  or double click on the unit parameter.




The most commonly used attributes of a unit parameter are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed unit parameters. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``DEFINITION`` : The ``DEFINITION``  attribute can (and should) be used to specify a unit expression. In case the unit expression is a constant unit expression (e.g. ``[m]`` ), there is in fact no need for a unit parameter and the unit ``[m]``  could be directly specified as the unit attribute of the corresponding identifiers.




**Remark** 


To be able to declare a unit parameter your model has to be equipped with at least one quantity identifier. 





**How to ...** 

*	:ref:`Model-Explorer_Creating_a_Quantity`  




**Learn more about** 

*	:ref:`sec:units.unit-par`  
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



