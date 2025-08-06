

.. _Curve_Object_Properties_-_Visible:


Visible
=======

**Description** 

On the Visible tab you can specify whether an object should be visible or hidden on the page when it is in user mode.

Although you can specify that an object is hidden at all times, you will usually specify the hidden status via a scalar identifier. If the value of this identifier is not equal to 0, then the object will be hidden.



**Identifier Hidden (table only)** 

If you do not make the entire table hidden, you can specify that only some of the contained identifiers in the table must be hidden. To make an identifier in the table hidden, you can enter the value 1 in the corresponding field. But, if you want to let the hidden status depend on a value in your model you can also specify a scalar.



**Tips & Tricks** 

*	Using the visibility properties of an object, you can create a page where you alternatively show different (type of) objects within the same area of the page. For example, you can create a bar chart and a table object on exactly the same position on your page, and let the user select which one he prefers to see.
*	If you want to hide a whole group of objects, then (as an alternative for specifying the visibility status for each object) you can also choose to put these objects on a separate template. With the Hidden property of this template you can determine whether these objects should be visible or not. Note however, that this Hidden property of a template is only checked when the page is created, and changing it while the page is already opened has no effect.
*	If your project is linked to a user database and contains Authorization Levels, you can use the value of the pre-defined identifier CurrentAuthorizationLevel to determine whether the current user is allowed to view an object.



