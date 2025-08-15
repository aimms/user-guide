

.. _Model-Explorer_Changing_the_Node_Type:


Change the Node Type
====================

**Description** 

Some groups of identifier types are quite similar with respect to either their use within a model or with respect to the set of available attributes. For identifiers of such type, AIMMS allows you to modify the identifier type to another type within that same group. For example, you can change a string parameter to a unit parameter, a parameter to a variable, a set to a horizon, etc.

To change the type of an identifier:

1.	Select the identifier in the Model Tree

2.	From the Edit menu, select Change Type

If there are any compatible identifier types for the selected identifier, a dialog box will appear. In this dialog box:

3.	Select the new identifier type

4.	Click OK



Not all compatible identifier types have the same set of allowed attribute values. If, by changing the identifier type, a specific already specified attribute is not allowed in the new type, then the dialog box will list this attribute. If you confirm the change (by clicking OK), these attribute values will be deleted.



You can also change the identifier type from within the attribute form of the identifier. At the top of the attribute form a special combo box lists all possible compatible identifier types, and allows you to simply select the new type.



