

.. _Diagnostic-Tools_Identifier_Cardinalities:


Identifier Cardinalities
========================

**Description** 

By selecting Diagnostic Tools – Identifier Cardinalities from the Tools menu, you will open the Identifier Cardinalities dialog box. The following information is displayed for each identifier:

*	Cardinality – the total number of non-default values currently stored,
*	Maximal cardinality – the cardinality if all values would assume a non-default value,
*	Density – the cardinality as a percentage of the maximal cardinality,
*	Active – the number of elements, with non-default value, that lie within the domain of the identifier, and
*	Inactive – the number of elements, with non-default value, that lie outside of the domain of the identifier.
*	Mem Usage – the total amount of memory used by the identifier.




You can locate potential dense data storage problems by sorting all identifiers by their cardinality. Identifiers with a very high cardinality and a high density can indicate a missing or incorrectly specified domain condition.





**Note** 

*	Realize that AIMMS also uses identifiers that are not visible as identifiers in the model tree. By selecting the "Show predeclared identifiers" property, the identifier cardinalities dialog will also show information for predeclared identifiers, by selecting the "Show Identifier Suffices" the dialog will also show information for identifiers that AIMMS declares for, for example, index domain conditions. A list of all predeclared identifiers can be found in the function reference.



