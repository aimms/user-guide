.. _ODH-CPLEX_XCuts_-_MIP_Nr_of_Cut_Pa:


MIP Number of Cut Passes
========================



:Type:	Integer	
:Range:	{-1 .. 2147483647}	
:Default:	0	



The option sets the upper limit on the number of passes CPLEX performs when generating cutting planes of a MIP model. At the default setting of 0, CPLEX decides. If the value is -1 then CPLEX performs no passes. Strictly positive values give the number of passes to perform.



