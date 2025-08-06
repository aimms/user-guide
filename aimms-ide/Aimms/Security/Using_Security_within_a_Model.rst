

.. _Security_Using_Security_within_a_Model:


Using Security within a Model
=============================

**Description** 

To adjust your model and pages and make use of the users settings and authorization levels, you can refer to three predefined parameters:

*	``CurrentUser`` , a string parameter containing the name of the current user,
*	``CurrentGroup``  a string parameter containing the name of the smallest group to which the current user belongs, and
*	``CurrentAuthorizationLevel`` , an element parameter containing the authorization level of the current user.




These predefined AIMMS parameters cannot be changed from within your model. Their value can only be changed using the user security features from AIMMS.





Using the User Setup Tool the User Administrator can associate one of the available authorization levels with every user. When such a particular user logs on, the predefined AIMMS element parameter ``CurrentAuthorizationLevel``  will be set to his/her specified authorization level. Depending on this value the model developer can

*	Decide whether or not to allow execution of a procedure,
*	Enable or disable page objects or menu items.




**How to** 

*	:ref:`Security_Changing_User_within_an_Applic`  
*	:ref:`Security_Changing_Group_within_an_Appli`  
*	:ref:`Security_Changing_Authorization_Level_w`  
*	:ref:`Security_Enumerating_Users_and_User_Gro`  




**Learn more about** 

*	:ref:`Menu-Builder_Menu_node_properties_control`  



