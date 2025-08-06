

.. _Scalar_Object_Properties_-_Input:


Input
=====

**Description** 

On the Input tab of the properties dialog box, you can define whether the user should be able to change values within the object. With the properties on this tab you can set a read-only status for either the entire object, or for some individual identifiers that are contained in the object.



**Object Read-Only** 

You can set the entire object in a read-only state, so that none of the displayed values can be changed by the user. However, the user can still browse and scroll through the data in the object, or select a specific entry. If you want to let the read-only status of an object depend on a value in your model, you can specify the read-only status via a scalar identifier. If the value of this identifier is not equal to 0, then the object is read-only.



**Identifier Read-Only** 

If you do not make the entire object read-only, you can specify that only some of the contained identifiers in the object must be read-only. To make an identifier in the object read-only, you can enter the value 1 in the corresponding field. But, if you want to let the read-only status depend on a value in your model you can also specify a scalar or multi-dimensional identifier. Then, the identifier contained in the object is read-only if the value of this specified identifier is not equal to 0. If you specify a multi-dimensional identifier (with a domain that matches the domain of the identifier contained in the object), you can specify a read-only status for the individual entries of that identifier.



**Note** 

*	With the Input properties, you can only narrow down which objects and identifiers are still updatable on a page. Thus, if the model defines that an identifier is not updatable, toggling the read-only status has no effect.




**Learn more about** 

*	:ref:`Miscellaneous_Updatebility_of_Identifiers` 



