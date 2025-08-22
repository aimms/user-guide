.. |img_def_Identifier_Parameter_bmp| image:: images/Identifier_Parameter.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Parameter:


Creating a Parameter
====================

**Description** 

To create a new parameter in the Model Tree:

1.	Select the position in a Declaration Section where the new parameter should be inserted

2.	From the Edit menu select Insert – Parameter |img_def_Identifier_Parameter_bmp|

3.	Enter a name for the new parameter (if you are creating a multi-dimensional parameter, you can type the indices of each dimension as well)

4.	Press ``<Enter>``  to create the new parameter (or press ``<Esc>``  to abort the operation)



The newly created parameter is now ready for use, but you probably want to specify some additional attributes. To modify the attributes of the newly created parameter:

*	Press ``<Enter>``  or double click on the parameter node.




The most commonly used attributes of a parameter are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed parameters. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``RANGE``  : The ``RANGE``  attribute should be specified in order to restrict the values to certain intervals. The |img_def_Wizard_button_bmp| wizard will let you either select one of the predefined ranges, like ``Real`` , ``Nonnegative`` , ``Nonpositive`` , ``Integer`` , or ``Binary`` , or specify a (parametric) interval range.
*	``UNIT``  : The ``UNIT``  attribute is used to specify the unit in which the parameter value is measured. By specifying a unit, AIMMS is able to perform automatic unit conversions and unit consistency checks. The |img_def_Wizard_button_bmp| wizard will let you select a unit and quantity from the list made up from your model quantities and units together with the information in the AIMMS SI unit base.
*	``DEFAULT``  : The ``DEFAULT``  attribute should be used in order to specify a nonzero default value for the parameter. Note that AIMMS will explicitly store all values that are non-default. 
*	``DEFINITION`` : The ``DEFINITION``  attribute can (and should) be used to specify the definition of an identifier by means of a global relationship. AIMMS stores the result of a definition and recomputes it only when necessary.




**Learn more about** 

*	:ref:`sec:par.decl` 
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`sec:nonproc.dep`  



