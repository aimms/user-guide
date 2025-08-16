

.. _Options_Startup__authorization_-_Inter:


Interrupt Procedure
===================



:Type:	Name of a procedure	
:Default:	\-	



This option specifies the procedure that is executed when the user tries to interrupts a procedure run via <Ctrl>-<Shift>-<S>. If you allow the end-user to interrupt the run at the current stage of the run, the procedure must return a non-zero value. If you do not specify this procedure, the end-user can interrupt the current run at any time. By specifying your own interrupt procedure you make sure that the user can only interrupt a procedure at certain stages of the execution, and thus prevent the model to be left in an undetermined state.



**Note** 

*	When no procedure is selected (the default), AIMMS asks for a confirmation before interrupting.
*	If an interrupt procedure returns 1, then AIMMS will stop after executing the procedure. In case the procedure returns 0, AIMMS will continue after executing the procedure.




**Tips & Tricks** 

*	You can interrupt AIMMS by pressing <Ctrl>+<Shift>+S.




**Learn more about** 

*	:ref:`Model-Explorer_Procedures`  



