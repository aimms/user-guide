

.. _option-AIMMS-enhanced_long_run_responsiveness:


Enhanced Long Run Responsiveness
================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



With this option you can change the responsiveness of AIMMS during long execution runs. During long runs, AIMMS periodically checks the Windows message queue to see (amongst others) whether it needs to update parts of the screen or whether the Interrupt Run shortcut key has been pressed.

Until the release of Windows Vista, AIMMS did not suffer from any problems using this approach. However, this approach does not seem to be compatible with how Vista handles its running applications.

Using the normal (old) way in which AIMMS handles the messages during a long run, after some seconds, Vista decides that AIMMS is "not responding" and from thereon no messages get processed at all, resulting in (for example) a Progress Window that is not showing any more progress (although the run itself continues normally).



This option offers a work-around for this problem. When set to 'Yes', AIMMS tries to handle much more messages during a run.  However, a problem might be that AIMMS becomes too responsive, because a focus event could perhaps result in unwanted interaction during the run. The advise remains to not 'click-around' while AIMMS is busy running a long task.



Possible values are:



    *	Automatic 
    *	Yes
    *	No




The value 'Automatic' means that the option is set to 'Yes' on Vista based systems, and set to 'No' on non-Vista based systems.

