

.. _Security_Enumerating_Users_and_User_Gro:


Enumerating Users and User Groups
=================================

**Description** 

AIMMS does not provide predefined sets containing all the users and groups defined in the User Database linked to a project. However, if you need access to the set of all users and user groups in your application, AIMMS offers the following two functions to obtain this information.

*	``SecurityGetUsers(``  user-set [,group] [,level] ``)`` 
*	``SecurityGetGroups(``  group-set ``)`` 




The argument group is a string, the argument level an element in the set ``AllAuthorizationLevels`` , while the output arguments user-set and group-set must be set-identifiers.





When specified in a call to ``SecurityGetUsers``  the group and level arguments serve as filters, filling user-set with only those users names that are member of the given group and/or posses the given authorization level.





**Learn more about** 

*	 Search for SecurityGetUsers (Function Reference)
*	 Search for SecurityGetGroups (Function Reference)



