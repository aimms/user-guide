

.. _Options_Show_Stochastic_Data_if_Available:


Show Stochastic Data if Available
=================================

**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Never



When you are developing a stochastic programming model, it is often needed to inspect the stochastic data of the variables and parameters in your model. With this option you can define that a data page of a variable or parameter automatically shows the stochastic data (instead of the level data). Please note that if you have saved a data page for a specific identifier before, then this option has no effect and just the saved data page is stored.



Tip: Hold down the Shift key when requesting a data page, to ignore any previously saved data page.



Possible values are:



*	Never
*	Only Variables
*	Only Parameters
*	Both Variables and Parameters




If this option is set to a value other than the default then, in case stochastic data is present, AIMMS will show a dialog asking you whether you want to see the deterministic or stochastic values of a variable or parameter on a data page. This dialog will show the cardinalities of both the deterministic and stochastic data, to make the choice easier.





**Learn more about** 

*	:ref:`Page-Manager_Data_Page` 
