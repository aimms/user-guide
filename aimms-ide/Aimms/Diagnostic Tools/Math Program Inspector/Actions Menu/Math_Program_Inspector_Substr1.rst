

.. _Diagnostic-Tools_Math_Program_Inspector_Substr1:


Substructure Causing Infeasibility
==================================

**Description** 

To find that part of the model that is responsible for the infeasibility, slack variables are used. By default, the math program inspector adds slacks to all variable and constraint bounds with the exception of 

*	variables that have a definition,
*	zero variable bounds, and
*	bounds on binary variables.

The last two exceptions can be overruled at the symbolic level through the Analysis Configuration tab of the Properties dialog. Of course, by not allowing slack variables on all variable and constraint bounds in the model, it is still possible that the infeasibility will not be resolved.





After adding slack variables, this adapted version of the model is referred to as the elastic model. When looking for the substructure that causes infeasibility, the sum of all slack variables is minimized. All variables and constraints that have positive slack in the optimal solution of this elastic model, form the substructure causing the infeasibility. This substructure will be bookmarked in the variable and constraint tree.





**Learn more about** 

*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Bookmar` 
*	:ref:`Diagnostic-Tools_Math_Program_Inspector_Tree_Vi`  
*	Search for AIMMS math program inspector (User's Guide)






