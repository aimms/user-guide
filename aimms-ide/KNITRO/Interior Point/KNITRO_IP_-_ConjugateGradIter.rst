.. _KNITRO_IP_-_ConjugateGradIter:


Conjugate Gradient Iteration Limit
==================================



**Type**:	Integer	

**Range**:	{0..1000000}	

**Default**:	-1	



This option determines the maximum allowable number of inner conjugate gradient (CG) iterations per Knitro minor iteration. Possible values are: 



-1:    Knitro automatically determines an upper bound on the number of allowable CG iterations.

0:	Knitro will set an upper bound on the number of allowable CG iterations based on the problem size.	

n:	At most n>0 CG iterations may be performed during one Knitro minor iteration.



