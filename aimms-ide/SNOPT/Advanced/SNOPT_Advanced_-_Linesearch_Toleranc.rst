.. _SNOPT_Advanced_-_Linesearch_Toleranc:


Linesearch Tolerance
====================



**Type** :	Floating point number	

**Range** :	[0,1]	

**Default** :	0.9	



This option determines the accuracy with which a steplength will be located along the direction of search each iteration. At the start of each line search a target directional derivative for the merit function is identified. This option determines the accuracy to which this target value is approximated. The default value of 0.9 requests just moderate accuracy in the line search.



If the nonlinear functions are cheap to evaluate, a more accurate search may be appropriate; try 0.1, 0.01 or 0.001. The number of major iterations might increase.



If the nonlinear functions are expensive to evaluate, a less accurate search may be appropriate. If all gradients are known, try 0.99. (The number of major iterations might increase, but the total number of function evaluations may decrease enough to compensate.)



