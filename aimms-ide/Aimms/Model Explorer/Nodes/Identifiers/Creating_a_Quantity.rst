.. |img_def_Identifier_Quantity_bmp| image:: images/Identifier_Quantity.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Quantity:


Creating a Quantity
===================

**Description** 

To create a new quantity in the Model Tree:

1.	Select the position in a Declaration Section where the new quantity should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Quantity_bmp| Quantity and press OK

4.	Press <Enter> to select a pre-defined SI quantity using the Quantity wizard, or enter your own quantity name and press <Enter>.



The quantity wizard displays a set of predefined AIMMS SI quantities. When selecting a quantity in the quantity wizard, the ``BASE UNIT``  attribute and the ``COMMENT`` attribute are filled with common choices corresponding to the selected quantity (e.g. the base unit of the quantity 'SI_Length' will be set to 'm'). To specify the attributes of the newly created quantity, you should 

*	Press ``<Enter>``  or double click on the quantity.




The most commonly used attributes of a quantity are discussed below. 




*	``BASE UNIT``  : The ``BASE UNIT``  attribute is mandatory and is used to specify the base unit for the current quantity. All internal AIMMS and case data are expressed in terms of the base unit. For this reason the base unit should be chosen to the unit in which most model quantities are measured. For example, if all lengths in your model are measured in terms of ``[km]`` , you are advised to make ``[km]``  the base unit of the quantity 'Length' (instead of ``[m]`` ). The |img_def_Wizard_button_bmp| wizard will display a list of all units that are commensurate with the current base unit.
*	``CONVERSION``  : The ``CONVERSION``  attribute is used to specify derived units. For any derived unit, you must specify a linear relation between the derived unit and the base unit. The |img_def_Wizard_button_bmp| wizard will display a dialog box containing a number of predefined conversions (for the common SI quantities). The wizard will also help you specify new conversions.




**How to ...** 

*	:ref:`Model-Explorer_Creating_New_Nodes`  




**Learn more about** 

*	:ref:`sec:units.quantity`  
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



