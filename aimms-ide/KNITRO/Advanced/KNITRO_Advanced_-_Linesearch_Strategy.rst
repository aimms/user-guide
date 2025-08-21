.. _option-KNITRO-linesearch_strategy:


Linesearch Strategy
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option indicates which linesearch strategy to use for the Interior-Direct or SQP algorithm to search for a new acceptable iterate. Possible values are:



*	Automatic
*	Backtrack
*	Interpolate
*	Weak Wolfe Line search (unconstrained only)




This option has no effect on the Interior-CG or Active-Set algorithm.





**Learn more about** 

*	:ref:`option-KNITRO-algorithm` 
