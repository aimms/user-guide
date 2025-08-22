.. |img_def_Identifier_Convention_bmp| image:: images/Identifier_Convention.bmp


.. _Model-Explorer_Creating_a_Convention:


Creating a Convention
=====================

**Description** 

To create a new convention in the Model Tree:

1.	Select the position in a Declaration Section where the new convention should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Convention_bmp| Convention and press OK

4.	Enter a name for the new convention

5.	Press ``<Enter>``  to create the new (or press ``<Esc>``  to abort the operation)



The newly created convention is now ready for use, but you probably want to specify some additional attributes. To modify the attributes of the newly created convention:

*	Press ``<Enter>``  or double click on the convention.




The most commonly used attributes of a convention are discussed below. 




*	``PER QUANTITY``  : The ``PER QUANTITY``  attribute should be used to override the unit of all identifiers that express a value of a particular quantity. For example, if the ``PER QUANTITY``  attribute contains a line ``'SI_LENGTH : inch`` ', all identifiers that are expressing a length (and were expressed in terms of ``[m]`` , ``[cm]`` , ``[mile]`` , etc.), will be expressed in ``[inch]`` .
*	``PER UNIT``  : The ``PER UNIT``  attribute should be used to override the unit of all identifiers that share a particular ``UNIT``  attribute. For example, if the ``PER UNIT``  attribute contains a line '``m : cm`` ', all identifiers that are originally measured in ``[m]``  will be expressed in ``[cm]`` , and all identifiers that are originally measured in ``[m/s]``  are expressed in ``[cm/s]``  etc.
*	``PER IDENTIFIER``  : The ``PER IDENTIFIER``  attribute should be used to override the unit of a particular identifier. By applying the convention. For example, if the ``PER IDENTIFIER``  attribute contains a line '``Size : m`` ', the identifier '``Size`` ' will be expressed in terms of ``[m]``  (assumed that its original ``UNIT``  attribute was commensurate with ``[m]`` ).

**How to ...** 

*	:ref:`Model-Explorer_Creating_New_Nodes`  

**Learn more about** 

*	:ref:`sec:units.convention`
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



