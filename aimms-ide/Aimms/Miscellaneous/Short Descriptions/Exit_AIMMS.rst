.. |img_def_Close_Window_button_bmp| image:: images/Close_Window_button.bmp


.. _Miscellaneous_Exit_AIMMS:


Exit AIMMS
==========

**Description** 

As with most standard windows applications, there are two ways of exiting AIMMS, by selecting Exit from the File menu, or by selecting the cross button |img_def_Close_Window_button_bmp| in the upper right corner of the AIMMS window.



**Note** 

*	When a project is open when you exit AIMMS, the procedure MainTermination will be run before you exit the project. In this procedure you can include the statements that should always be executed before a user is allowed to exit the project (for example the statements for saving the modified data). The procedure MainTermination should return a nonzero value to allow the user to close the project, otherwise the project is not closed.




**Learn more about** 

*	:ref:`Miscellaneous_MainTermination`  



