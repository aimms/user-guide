.. |img_def_Identifier_Assertion_bmp| image:: images/Identifier_Assertion.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_an_Assertion:


Creating an Assertion
=====================

**Description** 

To create a new assertion in the Model Tree:

1.	Select the position in a Declaration Section where the new assertion should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Assertion_bmp| Assertion and press OK

4.	Enter a name for the new assertion (if you are creating an indexed assertion, you can type the indices as well)

5.	Press ``<Enter>``  to create the new assertion (or press ``<Esc>``  to abort the operation)



The newly created assertion is not yet ready for use, because you should at least specify its definition attribute. To modify the attributes of the newly created assertion:

*	Press ``<Enter>``  or double click on the assertion node.




The most commonly used attributes of an assertion are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed assertions. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``DEFINITION``  : The ``DEFINITION``  attribute should contain a logical expression that is to be verified when the assertion is executed.
*	``ACTION``  : The ``ACTION``  attribute is used to specify some non-default action (by default a message box with displaying the contents of the ``TEXT``  attribute is displayed), that is performed when the assertion fails. The ``ACTION``  attribute is comparable to a ``BODY``  attribute of an AIMMS function or procedure.




**Learn more about** 

*	:ref:`sec:data.assert`
*	:ref:`Model-Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



