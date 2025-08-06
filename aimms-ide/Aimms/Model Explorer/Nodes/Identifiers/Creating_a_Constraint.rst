.. |img_def_Identifier_Constraint_bmp| image:: images/Identifier_Constraint.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Constraint:


Creating a Constraint
=====================

**Description** 

To create a new constraint in the Model Tree:

1.	Select the position in a Declaration Section where the new constraint should be inserted

2.	From the Edit menu select Insert – Constraint |img_def_Identifier_Constraint_bmp|

3.	Enter a name for the new constraint (if you are creating a multi-dimensional constraint, you can type the indices of each dimension as well)

4.	Press ``<Enter>``  to create the new constraint (or press ``<Esc>``  to abort the operation)



The newly created constraint is not yet ready for use, because you should at least specify the definition of a constraint via its attributes. To modify the attributes of the newly created constraint:

*	Press ``<Enter>``  or double click on the constraint node.




The most commonly used attributes of a constraint are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed constraints. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``UNIT``  : The ``UNIT``  attribute is used to specify the unit in which the constraint's RHS value is measured. By specifying a unit, AIMMS is able to perform automatic unit conversions and unit consistency checks. The |img_def_Wizard_button_bmp| wizard will let you select a unit and quantity from the list made up from your model quantities and units together with the information in the AIMMS SI unit base.
*	``PROPERTY`` : The ``PROPERTY``  attribute should be used to specify additional properties. Note that in order to retrieve sensitivity information from the solver, the ``ShadowPrices`` , ``RightHandSideRange`` , or ``ShadowPriceRange``  property should be explicitly set. The |img_def_Wizard_button_bmp| wizard will let you specify the properties through a selection of radio buttons and check boxes.
*	``DEFINITION`` : The ``DEFINITION``  attribute is mandatory and should contain the constraint formulation containing two or three expressions separated by one of the relational operators ``=`` , ``<=`` , or ``>=`` .




**Learn more about** 

*	Search for Constraint and constraint attributes (Language Reference)
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



