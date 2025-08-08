.. |img_def_Identifier_Arc_bmp| image:: images/Identifier_Arc.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_an_Arc:


Creating an Arc
===============

**Description** 

To create a new arc in the Model Tree:

1.	Select the position in a Declaration Section where the new arc should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Arc_bmp| Arc and press OK

4.	Enter a name for the new arc (if you are creating a multi-dimensional arc, you can type the indices of each dimension as well)

5.	Press ``<Enter>``  to create the new arc (or press ``<Esc>``  to abort the operation)



The newly created arc is not yet ready for use, because you should at least specify some mandatory attributes. To modify the attributes of the newly created arc:

*	Press ``<Enter>``  or double click on the arc node.




The most commonly used attributes of an arc are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed arcs. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``RANGE``  : The ``RANGE``  attribute should be specified in order to restrict the values to certain intervals. The |img_def_Wizard_button_bmp| wizard will let you either select one of the predefined ranges, like ``Real`` , ``Nonnegative`` , ``Nonpositive`` , ``Integer`` , or ``Binary`` , or specify a (parametric) interval range.
*	``UNIT``  : The ``UNIT``  attribute is used to specify the unit in which the arc's value is measured. By specifying a unit, AIMMS is able to perform automatic unit conversions and unit consistency checks. The |img_def_Wizard_button_bmp| wizard will let you select a unit and quantity from the list made up from your model quantities and units together with the information in the AIMMS SI unit base.
*	``FROM``  : The ``FROM``  attribute is mandatory an should contain a node reference specifying the start node of the arc. The |img_def_Wizard_button_bmp| wizard will display an Identifier Selection Dialog box that helps you select the appropriate node.
*	``TO``  : The ``TO``  attribute is mandatory an should contain a node reference specifying the end node of the arc. The |img_def_Wizard_button_bmp| wizard will display an Identifier Selection Dialog box that helps you select the appropriate node.
*	``COST`` : The ``COST``  attribute is used to specify the cost coefficient that will be used to calculate the predefined AIMMS variable ``FlowCost`` . 
*	``PROPERTY`` : The ``PROPERTY``  attribute should be used to specify additional properties. Note that in order to retrieve sensitivity information from the solver, the ``ReducedCosts`` , ``ValueRange`` , or ``CoefficientRange``  property should be explicitly set. The |img_def_Wizard_button_bmp| wizard will let you specify the properties through a selection of radio buttons and check boxes.




**Remark** 


Arcs are used to formulate network models and are considered to be variables when it comes to solving the network model. 





**Learn more about** 

*	:ref:`sec:net.arc`
*	:ref:`Model-Explorer_Attribute_Forms` 
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`Miscellaneous_Identifier_Selection_Dialog_Bo`  



