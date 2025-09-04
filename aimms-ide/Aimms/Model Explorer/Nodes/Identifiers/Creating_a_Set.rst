.. |img_def_Identifier_Set_bmp| image:: images/Identifier_Set.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Set:


Creating a Set
==============

**Description** 

To create a new set in the Model Tree:

1.	Select the position in a Declaration Section where the new set should be inserted

2.	From the Edit menu select Insert – Set |img_def_Identifier_Set_bmp|

3.	Enter a name for the new set (if you are creating an indexed set, you can type these indices as well)

4.	Press ``<Enter>``  to create the new set (or press ``<Esc`` > to abort the operation)



The newly created set is now ready for use, but you probably want to specify some additional attributes (for example the indices in the set). To modify the attributes of the newly created set:

*	Press ``<Enter>``  or double click on the set node.




The most commonly used attributes of a set identifier are discussed below. 




*	``INDEX DOMAIN``: The ``INDEX DOMAIN`` attribute should be specified in order to declare indexed sets. However, in most models scalar, simple (or compound) sets suffice to formulate your model. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``SUBSET OF``: The ``SUBSET OF`` attribute should be specified in order to declare a subset. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more sets.
*	``INDEX``: The ``INDEX`` attribute is the most natural place to declare indices in the current set. The |img_def_Wizard_button_bmp| wizard allows you to declare a new index, delete or rename an existing index or move an index to another set. When declaring an index this way, the index is bound to the corresponding set. To declare an index that is not bound, you should explicitly declare an index identifier.
*	``PARAMETER``: The ``PARAMETER`` attribute is like the ``INDEX`` attribute except that it allows you to declare scalar element parameters (instead of indices) in the current set. Another common way to achieve the same is to explicitly declare an element parameter.
*	``DEFINITION``: The ``DEFINITION`` attribute can (and should) be used to specify the definition of an identifier by means of a global relationship. AIMMS stores the result of a definition and recomputes it only when necessary.




**How to ...** 

*	:ref:`Model-Explorer_Creating_an_Index`  
*	:ref:`Model-Explorer_Creating_an_Element_Parameter`  




**Learn more about** 

*	:ref:`sec:set.decl` 
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms` 
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  
*	:ref:`sec:nonproc.dep`  



