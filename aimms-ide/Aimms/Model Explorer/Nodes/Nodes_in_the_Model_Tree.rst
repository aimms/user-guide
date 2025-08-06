

.. _Model-Explorer_Nodes_in_the_Model_Tree:


Nodes in the Model Tree
=======================

**Description** 

The Model Tree lets you store information of different nature, such as identifier declarations, procedures, functions, and model sections. Each piece of information is stored as a separate node in the tree, and each node has its own type-dependent icon. 



The following table shows the allowed parent-child relations for the different main types of nodes in the Model Tree. When adding, moving or copying nodes, AIMMS will check these relations and prevent you from creating an invalid tree structure.




.. list-table::

   * -             ParentChild
     - Root
     - module section
     - book section
     - declaration section
     - procedure & function
     - identifier
   * - Module section
     - Ö
     - Ö
     - Ö
     - 
     - 
     - 
   * - Module section
     - Ö
     - Ö
     - Ö
     - 
     - Ö
     - 
   * - declaration section 
     - Ö
     - Ö
     - Ö
     - 
     - Ö
     - 
   * - procedure & function
     - Ö
     - Ö
     - Ö 1)
     - 
     - 
     - 
   * - Identifier	
     - 
     - 
     - 
     - Ö
     - 
     - 




1)	Nested procedures are not allowed.



**Learn more about** 

*	:ref:`Model-Explorer_Structuring_Nodes`  
*	:ref:`Model-Explorer_Identifier_Nodes`  
*	:ref:`Model-Explorer_Procedure_and_Function_Nodes`  



