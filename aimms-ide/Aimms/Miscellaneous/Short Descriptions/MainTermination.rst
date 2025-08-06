

.. _Miscellaneous_MainTermination:


MainTermination
===============

**Description** 

MainTermination is one of the three standard procedures in the model tree. This procedure is called prior to closing the project. Default the procedure contains this AIMMS code:



``if ( CaseSaveAll( confirm:2 ) = 1 ) then`` 

``return 1;`` 

``else`` 

``return 0;`` 

``endif ;`` 



In this case, AIMMS will ask you to save your data whenever you want to exit your project and a change has been made to the data since the last time you saved it. If no data needs to be saved, or if the data has been saved properly then the procedure returns 1, indicating that AIMMS is allowed to close the project. If the user has canceled the dialog, then the procedure returns 0, and AIMMS will not close the project.



You can alter the contents of this procedure, but you should make sure that you return the proper value. If you return 0 (or omit any return statement), then AIMMS will not close the current project. To indicate that AIMMS should close the project you must return a nonzero value. For example, if you want to close the project without any check on unsaved data, then this procedure should have the body:



``return 1;`` 



**Note** 

*	If you remove the procedure MainTermination from your model, then when closing the project, AIMMS will perform default checks on unsaved data (similar to the default contents of the procedure MainTermination, described above). Thus, if you want to influence the way in which AIMMS checks for unsaved data when closing the project, you should not delete the procedure MainTermination, but alter its contents.




**Learn more about** 

*	:ref:`Miscellaneous_MainInitialization`  
*	:ref:`Miscellaneous_MainExecution`  






