.. _CPLEX_MIP_-_MIP_Kappa:


MIP Kappa
=========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option sets the strategy for CPLEX to gather statistics about the MIP Kappa of subproblems of a MIP. MIP Kappa summarizes the distribution of the condition number of the optimal bases CPLEX encountered during the solution of a MIP model. That summary may let you know more about the numerical difficulties of your MIP model. Computing the kappa of a subproblem has a cost. In fact, computing MIP kappa for the basis matrices can be computationally expensive and thus generally slows down the solution process of a problem. Possible values are:



*	Off
*	Automatic
*	Sample
*	Full




The setting 'Automatic' tells CPLEX generally not to compute MIP kappa, but in cases where the option **Numerical Emphasis**  is turned on, CPLEX computes MIP kappa for a sample of subproblems.





The setting 'Sample' leads to a negligible performance degradation on average, but can slow down the branch-and-cut exploration by as much as 10% on certain models. In practice, the setting 'Sample' is a good trade-off between performance and accuracy of statistics. 





The setting 'Full' leads to a 2% performance degradation on average, but can significantly slow the branch-and-cut exploration on certain models. If you need very accurate statistics, then use this setting.





The information is printed in the AIMMS Message Window. It is also printed in the CPLEX status file if the general solvers option **Solver Listing Messages**  is set to 'All' or 'Remark'. The CPLEX status file is named 'CPLEX 22.1.sta' and it is placed in the log directory of the AIMMS project.





If MIP Kappa is computed then AIMMS will print the following statistics:





*   percentage of numerically ill-posed simplex bases;
*   percentage of numerically unstable simplex bases;
*   percentage of numerically suspicious simplex bases;
*   percentage of numerically stable simplex bases;
*   score of numerical difficulties;
*   highest condition number encountered.




The following sections discuss these summary statistics in greater detail.





**Percentage of numerically ill-posed simplex bases** 





The percentage of numerically ill-posed simplex bases (condition number greater than 1e+14) among simplex bases encountered during the MIP solve.





**Percentage of numerically unstable simplex bases** 





The percentage of numerically unstable simplex bases (condition number between 1e+10 and 1e+14) among simplex bases encountered during the MIP solve.





**Percentage of numerically suspicious simplex bases** 





The percentage of numerically suspicious simplex bases (condition number between 1e+7 and 1e+10) among simplex bases encountered during the MIP solve.





**Percentage of numerically stable simplex bases** 





The percentage of numerically stable simplex bases (condition number less than 1e+7) among simplex bases encountered during the MIP solve.





**Score of numerical difficulties** 





A score of numerical difficulties for a MIP solve. The score is an aggregate of the fractions of ill-posed, unstable, and suspicious bases encountered during branch-and-cut. Specifically, the score is computed as the sum: 





   ill-posed + 0.3 * unstable + 0.01 * suspicious.


 


When this value deviates from 0, caution is advised. However, depending on your model, values of 0.03 or so may still not be of great concern. Your knowledge of the expected numerical quality of the model under consideration should influence your interpretation of the score of numerical difficulties.





**Highest condition number encountered** 





The highest condition number encountered during a MIP solve.





**Note** 

*	MIP Kappa cannot be computed if the option **MIP Method**  equals 'Barrier' or 'Sifting'.




**Learn more about** 

*	:ref:`CPLEX_MIP_-_MIP_Method` 
*	:ref:`CPLEX_General_-_NumericalEmphasis` 
*	:ref:`Options_Solver_Specific_-_Solver_List1`  
