.. |img_def_Identifier_Variable_bmp| image:: images/Identifier_Variable.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Variable:


Creating a Variable
===================

**Description** 

To create a new variable in the Model Tree:

1.	Select the position in a Declaration Section where the new variable should be inserted

2.	From the Edit menu select Insert – Variable |img_def_Identifier_Variable_bmp|

3.	Enter a name for the new variable (if you are creating a multi-dimensional variable, you can type the indices of each dimension as well)

4.	Press ``<Enter>``  to create the new variable (or press ``<Esc>``  to abort the operation)



The newly created variable is now ready for use, but you probably want to specify some additional attributes. To modify the attributes of the newly created variable:

*	Press ``<Enter>``  or double click on the variable node.




The most commonly used attributes of a variable are discussed below. 




*	``INDEX DOMAIN``: The ``INDEX DOMAIN`` attribute should be specified in order to declare indexed variables. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``RANGE``: The ``RANGE`` attribute should be specified in order to restrict the values to certain intervals. The |img_def_Wizard_button_bmp| wizard will let you either select one of the predefined ranges, like ``Real``, ``Nonnegative``, ``Nonpositive``, ``Integer``, or ``Binary``, or specify a (parametric) interval range.
*	``UNIT``: The ``UNIT`` attribute is used to specify the unit in which the variable's value is measured. By specifying a unit, AIMMS is able to perform automatic unit conversions and unit consistency checks. The |img_def_Wizard_button_bmp| wizard will let you select a unit and quantity from the list made up from your model quantities and units together with the information in the AIMMS SI unit base.
*	``DEFAULT``: The ``DEFAULT`` attribute should be used in order to specify a nonzero default value for the variable. Note that AIMMS will explicitly store all values that are non-default. 
*	``PROPERTY``: The ``PROPERTY`` attribute should be used to specify additional properties. Note that in order to retrieve sensitivity information from the solver, the ``ReducedCosts``, ``ValueRange``, or ``CoefficientRange`` property should be explicitly set. The |img_def_Wizard_button_bmp| wizard will let you specify the properties through a selection of radio buttons and check boxes.
*	``DEFINITION``: The ``DEFINITION`` attribute for variables can be used specify a constraint that defines the value of the variable. Instead of specifying the constraint explicitly and adding it the constraint set of the mathematical program, AIMMS will generate additional constraints based on the ``DEFINITION`` attribute as needed.




**Learn more about** 

*	:ref:`sec:var.var` 
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`sec:nonproc.dep`  



