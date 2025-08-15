

.. _Options_NonlinPres_-_DisplayInfyAnalys:


Display Infeasibility Analysis
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether the infeasibility analysis should be printed to the listing file in case the AIMMS Presolver detects that the model is infeasible. Possible values are:



*	On
*	Off




The information printed in the listing file is the constraint that appeared to be infeasible and all other constraints that the AIMMS Presolver used to reduce the bounds of the variables in this infeasible constraint. Also the reductions on the variable bounds in these constraints are shown. For example:





1	AIMMS presolve infeasibility analysis for the first solve of NLPModel.





2	c1 ..


3


4	+ [Nonlinear term]


5	+ 1 * x1 = 0 ;


	



.. list-table::

   * - 6
     - name
     - lower
     - 
     - upper
   * - 7
     - x2
     - -0.200
     - -> 0    
     - 0.200 
   * - 8
     - y
     - 0
     - -> 4.200
     - inf
   * - 9
     - [Nonlinear term]       
     - -inf 
     - 
     - 0
   * - 10
     - x1
     - 1
     - 
     - 8     









11	c2 ..


12


13	+ x1 + y <= 4 ; ``****``


	



.. list-table::

   * - 14
     - name
     - lower
     - upper
   * - 15
     - x1
     - 1
     - 8
   * - 16
     - y
     - 4.2
     - inf






The lines 11-16 show the constraint 'c2' for which the AIMMS Presolver found an inconsistency. The variables 'x1' and 'y' can never be lower than 1 and 4.2 respectively and therefore the sum of these variables must be greater than or equal to 5.2 which contradicts the right hand side value of 4 of constraint 'c2'. The lower bound for variable 'y' was derived by the AIMMS Presolver from constraint 'c1' as shown in the lines 2-10. The original lower bound of variable 'y' was 0. The AIMMS Presolver also derived that the lower bound of variable 'x2' could be tightened from -0.2 to 0, but variable 'x2' was not (directly) responsible for the inconsistency.





**Note** 

*	The amount of information displayed for the infeasibility analysis can be large and might not be useful.






