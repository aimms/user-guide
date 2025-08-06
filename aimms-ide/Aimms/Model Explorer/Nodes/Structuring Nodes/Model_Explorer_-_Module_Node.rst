

.. _Model-Explorer_Model_Explorer_-_Module_Node:


Module Node
===========

**Description** 

Modules are essentially sections with a separate namespace. Modules can be used to build an entire application on the basis of existing model components. A module section can contain other module sections, book sections, declaration sections, procedures and functions.

A section node in the model explorer can have the following attributes:



*	``SOURCE FILE``  : With the ``SOURCE FILE``  attribute you can specify that the contents of the section should not be saved as part of the main model file, but that you want to save it in a separate file. This is especially useful when you want to interchange parts of the model between two different versions of the same project. This attribute can only be changed using the accompanying wizard. Note that if the source file is in the project folder or a child folder, the relative position will be saved, in all other cases the absolute file position will be used. Take this into consideration when moving a project.
*	``PREFIX`` :In this field you must specify a module-specific prefix to be used in conjunction with the :: operator.
*	``PUBLIC`` : In this field you can specify a set of identifiers declared within the module, whose names should be made public.
*	``PROTECTED`` : In this field you can specify a subset of the identifiers specified in the Public attribute. The setting here overrides the setting in the Public attribute.
*	``COMMENT``  : In this field you can place any comment. A good idea is to give a short global description of the contents of the section for future reference.







**Learn more about** 

*	:ref:`Model-Explorer_Model_Explorer_-_Declaration_S`  
*	:ref:`Model-Explorer_Procedure_and_Function_Nodes`  
*	 Search for Module nodes (Language Reference)






