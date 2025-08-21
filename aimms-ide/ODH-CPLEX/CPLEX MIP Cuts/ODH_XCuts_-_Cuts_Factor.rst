.. _option-ODHCPLEX-cuts_factor:


Cuts Factor
===========



:Type:	Floating point number	
:Range:	[-1, inf)	
:Default:	-1	



This option limits the number of all cuts that can be added. The number of rows in the problem with cuts added is limited to the value of this option times the original number of rows. If the problem is presolved, the original number of rows is that from the presolved problem.



For values between zero and one (that is, in the range [0.0, 1.0]), CPLEX generates no cuts.



The default value of this option is -1 (that is, negative one). The default value -1 means that CPLEX dynamically adjusts the limit on the number of cuts added to the model.

