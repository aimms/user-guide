

.. _option-AIMMS-display_infeasibility_analysis:


Display Infeasibility Analysis
==============================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether the infeasibility analysis should be printed to the listing file in case the AIMMS Presolver
detects that the model is infeasible. Possible values are:

    *	On
    *	Off

The information printed in the listing file is the constraint that appeared to be infeasible and all other constraints that
the AIMMS Presolver used to reduce the bounds of the variables in this infeasible constraint. Also the reductions on the
variable bounds in these constraints are shown. For example:


.. code-block:: text
   :linenos:

    AIMMS presolve infeasibility analysis for the first solve of NLPModel. 

    c1 ..

         + [Nonlinear term]
         + 1 * x1 = 0 ;

         name               lower                upper
         x2                 -0.200  ->  0        0.200
         y                  0       ->  4.200    inf
         [Nonlinear term]   -inf                 0
         x2                 1                    8


    c2 .. 

         + x1 + y <= 4 ;  **** 

         name    lower    upper
         x1      1        8
         y       4.200    inf
 

The lines 15-21 show the constraint 'c2' for which the AIMMS Presolver found an inconsistency. The variables
'x1' and 'y' can never be lower than 1 and 4.2 respectively and therefore the sum of these variables must be greater
than or equal to 5.2 which contradicts the right hand side value of 4 of constraint 'c2'. The lower bound for variable
'y' was derived by the AIMMS Presolver from constraint 'c1' as shown in the lines 3-12. The original lower bound of
variable 'y' was 0. The AIMMS Presolver also derived that the lower bound of variable 'x2' could be tightened from
-0.2 to 0, but variable 'x2' was not (directly) responsible for the inconsistency.


**Note** 

*	The amount of information displayed for the infeasibility analysis can be large and might not be useful.






