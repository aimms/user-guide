

.. _Model-Explorer_Assertions:


Assertions
==========

**Description** 

In most modeling applications it is important to check the validity of input data prior to its use. For instance, in a transportation model it makes no sense to try and solve the model if the total demand exceeds the total supply. In general, data consistency checks guard against unexplainable or even infeasible model results. As a result, these checks are essential to obtain customer acceptance of your application. In rigorous model-based applications it is not uncommon that the error consistency checks form a significant part of the total model text. 

To provide you with a mechanism to implement data validity checks, AIMMS offers a special Assertion data type. With it, you can easily specify and verify logical conditions for all elements in a particular domain, and take appropriate action when you find an inconsistency. Assertions can be verified from within the model through the Assert statement, or from within a page object in the graphical user interface. An assertions check can also be an action from a button, navigation object or menu item.



**Learn more about** 

*	:ref:`sec:data.assert`
*	:ref:`Shared-Object-Properties_Object_Properties_-_Assert`  
*	:ref:`Button_Button_Properties_-_Actions`  
*	:ref:`Navigation_Navigation_Object_Properties_1`  
*	:ref:`Menu-Builder_Menu_Node_Properties_-_Actions`  






