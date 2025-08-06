.. _KNITRO_MIP_-_MIP_Method:


MIP Method
==========



**Type** :	Selection	

**Range** :	The settings listed below	

**Default** :	Automatic	



This option specifies which MIP method to use. Possible values are:



*	Automatic
*	Branch-and-bound
*	Hybrid Quesada-Grossman method
*	MISQP




The hybrid Quesada-Grossman method should only be used for convex nonlinear problems. This algorithm is based on the paper: I. Quesada and I.E. Grossmann, An LP/NLP Based Branch and Bound Algorithm for Convex MINLP Optimization Problems, Computers and Chemical Engineering 16 (1992), pp. 937-947.





The MISCP method uses a mixed-integer SQP method, and allows for non-relaxable integer variables.




