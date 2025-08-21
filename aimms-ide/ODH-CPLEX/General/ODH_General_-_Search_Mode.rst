.. _option-ODHCPLEX-search_mode:


Search Mode
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Optimal solution	



This option specifies the search mode. Possible values are:



*	Optimal solution
*	Feasible solution




With setting 'Optimal solution', the main CPLEX solver behaves as it would with a normal solve with CPLEX with the exception that the embedded ODH engine is also invoked. If an integer feasible solution has been loaded into ODH-CPLEX, it is used as the starting point. In this mode, the ODH engine hits one of its stopping criteria such as those controlled by the options **Time Limit** , **Objective Target**  or **Maximum Divisor Value** . Unless the **Time Limit**  criterion is hit by the ODH engine, the main CPLEX solver continues until one of its stopping criteria is met, namely the MIP gap is sufficiently small, or a resource limit (e.g., time, node or iteration limit) is hit. Therefore with default settings this mode will search for an optimal solution. This mode supports callback procedures and (normal) progress updates.





With setting 'Feasible solution', ODH-CPLEX will try to find a solution to the problem. If an integer feasible solution has been loaded into ODH-CPLEX, it is used as the starting point for the heuristic. If one has not been loaded the heuristic uses its own first-feasible method to find one, or uses CPLEX to find one according to the value set for option **First Feasible Heuristic** . In this mode, ODH-CPLEX terminates only when it hits one of its stopping criteria, the options **Time Limit**  or **Maximum Divisor Value** , or if it runs out of possible sub-model decompositions. Termination on the last criterion is rare.





**Note** 

*	The mode 'Feasible solution' does not support callback procedures. If it is selected then almost no progress updates will be passed to AIMMS.




**Learn more about** 

*	:ref:`option-ODHCPLEX-first_feasible_heuristic`  
*	:ref:`option-ODHCPLEX-maximum_divisor_value`  
*	:ref:`option-ODHCPLEX-objective_target`  
*	:ref:`Options_Stop_Criteria_-_Time_Limit`   (General solvers option)
