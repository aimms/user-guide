

.. _Pivot-Table_DisplayanIdentifierSubsetv:


Display an Identifier Subset versus a Fixed List of Identifiers
===============================================================

When creating a Pivot Table you, as the GUI designer, can select a fixed selection of explicit identifiers for the data to be displayed in the Pivot Table. A consequence of displaying a fixed selection of identifiers is that the end-user cannot change the contents of the Pivot Table. 



Alternatively, you can specify that the collection of identifiers to display in a Pivot Table corresponds to the identifiers in a given subset of the predeclared set AllIdentifiers. In this mode, you can give control to the end-user which identifiers to display in the Pivot Table by allowing the end-user to modify the contents of the identifier subset associated with the Pivot Table. 



Even when displaying a identifier subset, you as a developer can have some control over the identifiers that can be displayed in the Pivot table by carefully restricting the possible contents of the identifier subset. You can accomplish that by not letting the set be a subset of AllIdentifiers directly but rather a subset of a subset of AllIdentifiers, the contents of which is under your control.



You can choose the identifier subset mode by specifying an identifier subset in the **Implicit Identifiers**  property on the **Contents**  tab of the properties dialog box of the Pivot table.



**See Also** 




*   The :ref:`Pivot-Table_Contents`  tab



