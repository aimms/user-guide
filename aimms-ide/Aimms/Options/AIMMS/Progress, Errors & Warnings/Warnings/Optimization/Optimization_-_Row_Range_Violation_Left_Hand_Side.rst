

.. _Options_Optimization_-_Row_Range_Violation_Left_Hand_Side:


Row Range Violation Left Hand Side
==================================



Type:	Selection	

Range:	The settings listed below	

Default:	On	



At the end of the first generation of a mathematical program, individual constraints are checked for feasibility by computing the range of the left hand side and comparing it to the right hand side. 



As an example, consider the following constraint:



CONSTRAINT:

  identifier : gt3

  definition : b1 + b2 >= 3



Here b1 and b2 are binary variables. AIMMS issues the following error message for this constraint: "The range of the left hand side of the ">=" constraint gt3 is [0, 2], and the right hand side of that constraint is 3; this constraint is infeasible."



Possible values of this option are:



*	Off (do not check individual constraints for feasibility)
*	On (check individual constraints for feasibility)




**Note** 


*   When generating and solving a mathematical program are steps in a larger algorithm, such as Benders Decomposition or Outer Approximation, infeasibility is a valid outcome of a single step. This error message may cause such an algorithm to stop whilst it should continue after an infeasibility in a single step. For such applications, it may be useful to switch this option off.
*   The option **Row Range Violation Left Hand Side Tolerance**  specifies the tolerance used for this feasibility check.




**Limitations** 


*   This check is only applicable to constraints that contain a left and right hand side separated by one of the operators <, <=, =, >=, >.
*   It is not applied to special purpose constraints such as diversification filters.
*   It is not applied to constraint programming global constraints.
*   It is not applied to range constraints or if-then-else constraints.
*   It is not applied to constraints referencing if-then-else expression or external functions.




**See also** 


*   :ref:`Options_Optimization_-_Warning_Row_Range_Left_Hand_Side` 




**Learn more about** 


*   :ref:`Options_Warnings_-_Maximal_Number_of_W` 
*   :ref:`sec:exec.error`
*   :ref:`Options_Matrix_Generation_-_Row_Range_Violation_LHS_Tol` 

