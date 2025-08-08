.. |img_def_Identifier_Horizon_bmp| image:: images/Identifier_Horizon.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Horizon:


Creating a Horizon
==================

**Description** 

To create a new horizon in the Model Tree:

1.	Select the position in a Declaration Section where the new horizon should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Horizon_bmp| Horizon and press OK

4.	Enter a name for the new horizon

5.	Press ``<Enter>``  to create the new horizon (or press ``<Esc>``  to abort the operation)



The newly created horizon is not yet ready for use, because you should at least specify some mandatory attributes. To modify the attributes of the newly created horizon:

*	Press ``<Enter>``  or double click on the horizon node.




The most commonly used attributes of a horizon identifier are discussed below. 




*	``SUBSET OF`` : The ``SUBSET OF``  attribute should be specified in order to declare a subset. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more sets.
*	``INDEX`` : The ``INDEX`` attribute is the place to declare indices in the current horizon. The |img_def_Wizard_button_bmp| wizard allows you to declare new index, delete or rename an existing index or move an index to another set. 
*	``PARAMETER`` : The ``PARAMETER`` attribute is like the ``INDEX``  attribute except that it allows you to declare scalar element parameters (instead of indices) in the current horizon. 
*	``DEFINITION`` : The ``DEFINITION``  attribute is mandatory and should be used to determine the ordering of the periods in the horizon.
*	``CURRENT PERIOD`` : The ``CURRENT PERIOD``  attribute is used to specify the first period of the planning interval. The ``CURRENT PERIOD``  attribute together with the ``INTERVAL LENGTH``  attribute determine the generation of constraints and variables in your model. The |img_def_Wizard_button_bmp| wizard will display an Identifier Selection Dialog box containing all element parameters that are defined over the current horizon.
*	``INTERVAL LENGTH`` : The ``INTERVAL LENGTH``  attribute is used to specify the number of periods that should be considered during the model generation. If not specified, all periods from the current period onward are part of the planning interval.




**Remark** 


A horizon is a special kind of set. When variables and constraints are indexed over a horizon, AIMMS automatically restricts the generation of these constraints and variables to periods within the planning interval.





**How to ...** 

*	:ref:`Model-Explorer_Creating_a_Set`  




**Learn more about** 

*	:ref:`sec:time.horizon` 
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`Miscellaneous_Identifier_Selection_Dialog_Bo`  



