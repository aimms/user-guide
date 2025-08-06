

.. _Security_Unlinking_a_User_Database:


Unlinking a User Database
=========================

To remove a link between an existing User Database and an application

1.	From the Settings menu, open the User Setup submenu and select the UnLink command.

2.	Enter the User Administrator password



**Remark** 

Any cases and datasets in a project that is linked to a User Database, are owned by the specific user (and group) that created it. Therefore, there is a unique correspondence between a Data file and a User Database. If you unlink the current User Database from your project, you must decide how this affects you current Data file. There are two options:

1.	The owner reference for all cases and datasets in the current Data file is removed. After this, all cases and datasets can be accessed by any other user.

2.	You start with a new Data file. The current Data file will remain unchanged (keeping the owner references that belong to the 'old' User Database)

Similarly, if you try to open another existing Data file, this is only allowed if the owner references in this Data file match with the currently linked User Database.



