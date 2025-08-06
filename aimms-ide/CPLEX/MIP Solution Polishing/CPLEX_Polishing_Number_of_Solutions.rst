.. _CPLEX_Polishing_Number_of_Solutions:


Polishing Number of Solutions
=============================



**Type** :	Integer	

**Range** :	{1 .. 2147483647}	

**Default** :	2147483647	



This option sets the number of integer solutions to find before CPLEX stops branch-and-cut and begins to polish a feasible solution. The default value is such that CPLEX does not invoke solution polishing by default. 



CPLEX must have a feasible solution in order to start polishing. It must also have certain internal structures in place to support solution polishing. Consequently, when the criterion specified by this parameter is met, CPLEX begins solution polishing only after these starting conditions are also met. That is, there may be a delay between the moment when the criterion specified by this parameter is met and when solution polishing starts.



