.. _GUROBI_Hints:


Hints
=====

Gurobi 12.0 can use variable hints for MIP models. If you know that a variable is likely to take a particular value in high quality solutions of a MIP model, you can provide that value as a hint. You can also (optionally) provide a hint priority which resembles your level of confidence in a hint.



The Gurobi MIP solver will use these variable hints in a number of different ways. Hints will affect the heuristics that Gurobi uses to find feasible solutions, and the branching decisions that Gurobi makes to explore the MIP search tree. In general, high quality hints should produce high quality MIP solutions faster. In contrast, low quality hints will lead to some wasted effort, but shouldn't lead to dramatic performance degradations.



Variables hints and MIP starts are similar in concept, but they behave in very different ways. If you specify a MIP start, the Gurobi MIP solver will try to build a single feasible solution from the provided set of variable values. If you know a solution, you should use a MIP start to provide it to the solver. In contrast, variable hints provide guidance to the MIP solver that affects the entire solution process. If you have a general sense of the likely values for variables, you should provide them through variable hints.



Hint priorities are relative. If you are more confident in the hint value for one variable than for another, you simply need to set a larger priority value for the more solid hint. It is not necessary to specify a hint priority. In that case the default value of 0 will be used for the hint priority of the variable.



The hint value and hint priority can be set in the AIMMS project by using the function GMP::Solution::SetColumnValue. For example, to pass the current level values of the variable JobSchedule as hints you can use:



  myGMP := GMP::Instance::Generate( FlowShopModel );



  for (j,s) do

    GMP::Solution::SetColumnValue( myGMP, 1, JobSchedule(j,s), JobSchedule(j,s).level, 2 );

    GMP::Solution::SetColumnValue( myGMP, 1, JobSchedule(j,s), 10, 3 );

  endfor;



  GMP::Instance::Solve( myGMP );



In this example the hint priority for JobSchedule is set to 10.



Optionally, you can also read hints from a file, as controlled by the option **Hints File** .



**Learn more about** 

*	Search for GMP::Solution::SetColumnValue (Function Reference)
*	:ref:`GUROBI_MIP_-_Hints_File`  
