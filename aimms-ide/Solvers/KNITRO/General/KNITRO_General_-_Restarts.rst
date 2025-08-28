.. _option-KNITRO-restarts:


Restarts
========



:Type:	Integer	
:Range:	{1..1000000}	
:Default:	0	



This option specifies whether or not to enable automatic restarts in Knitro. When enabled, if a Knitro algorithm seems to be converging slowly or not converging, the algorithm will automatically restart, which may help with convergence. Possible values are: 



0:	No automatic restarts allowed.

n:	At most n automatic restarts may be performed.



