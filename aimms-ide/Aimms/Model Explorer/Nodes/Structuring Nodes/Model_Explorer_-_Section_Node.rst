.. |img_def_Section_Node_Open_bmp| image:: images/Section_Node_Open.bmp


.. _Model-Explorer_Model_Explorer_-_Section_Node:


Section Node
============

**Description** 

Book Section nodes are used to subdivide a model into logical parts with clear and descriptive names. Book sections are represented by a book icon that opens |img_def_Section_Node_Open_bmp| when the section is expanded. A book section can contain other book sections, module sections, declaration sections, procedures and functions.

A section node in the model explorer can have the following attributes:



*	``SOURCE FILE``: With the ``SOURCE FILE`` attribute you can specify that the contents of the section should not be saved as part of the main model file, but that you want to save it in a separate file. This is especially useful when you want to interchange parts of the model between two different versions of the same project. This attribute can only be changed using the accompanying wizard. Note that if the source file is in the project folder or a child folder, the relative position will be saved, in all other cases the absolute file position will be used. Take this into consideration when moving a project.
*	``COMMENT``: In this field you can place any comment. A good idea is to give a short global description of the contents of the section for future reference.







**Learn more about** 

*	:ref:`Model-Explorer_Model_Explorer_-_Module_Node`  
*	:ref:`Model-Explorer_Model_Explorer_-_Declaration_S`  
*	:ref:`Model-Explorer_Procedure_and_Function_Nodes`  






