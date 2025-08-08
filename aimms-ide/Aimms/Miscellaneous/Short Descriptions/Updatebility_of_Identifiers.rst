

.. _Miscellaneous_Updatebility_of_Identifiers:


Updatebility of Identifiers
===========================

**Description** 

Default identifiers with definitions are element of the predeclared AIMMS set, CurrentAutoUpdatedDefinitions, which means that whenever one of the identifiers in the definition changes value, the identifier will be updated.

You can choose to update identifiers that are not in the set CurrentAutoUpdatedDefinitions, when a change is made to one of the identifiers in the definition of the identifier. This can be done by filling the identifier name in the Update Upon Data Change field of the Procedure tab of the data object. 

Identifiers without definitions are default in the predeclared AIMMS set CurrentInputs, which means that both the model and the user is allowed to change the values of these identifiers. Identifiers that are not in the set CurrentInputs can not be changed in page objects regardless of the read-only state of the object.



**Learn more about** 

*	:ref:`Shared-Object-Properties_Object_Properties_Procedure`  
*	:ref:`Shared-Object-Properties_Object_Properties_-_Input`  
*	:any:`CurrentAutoUpdatedDefinitions`






