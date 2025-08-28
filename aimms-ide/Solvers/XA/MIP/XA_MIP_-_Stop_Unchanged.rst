.. _option-XA-stop_unchanged:


Stop Unchanged
==============



:Type:	Integer	
:Range:	{0..2100000000}	
:Default:	0	



This option determines the amount of time in seconds to continue the solution process after finding a new integer solution. If a new integer solution is not found in this time frame, then XA terminates. The reported integer solution may not be the optimal integer solution because of premature termination. The default value zero indicates no termination.



