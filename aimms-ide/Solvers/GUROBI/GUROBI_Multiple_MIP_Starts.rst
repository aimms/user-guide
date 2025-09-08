.. _GUROBI_Multiple_MIP_Starts:


Multiple MIP Starts
===================

Gurobi supports multiple MIP starts; that is, a user may maintain more than one starting solution with values for continuous and discrete variables for Gurobi to use as an advanced starting point. MIP starts are also known as advanced starts or warm starts.



A solution in the solution repository can be marked as a MIP start by using the AIMMS routine GMP::Solution::SetMIPStartFlag. For example, to mark the solutions 2 and 3 in the solution repository of a mathematical program 'MP' and solve the MIP use

.. code-block:: aimms

   gmpMP := GMP::Instance::Generate( MP );

   GMP::Solution::SetMIPStartFlag( gmpMP, 2, 1 );
   GMP::Solution::SetMIPStartFlag( gmpMP, 3, 1 );

   GMP::Instance::Solve( gmpMP );

where 'gmpMP' is an element parameter with range :aimms:set:`AllGeneratedMathematicalPrograms`.



**Note** 

*	The option **MIP Start**  can be used if only one MIP start is available.




**Learn more about** 

*	:any:`GMP::Solution::SetMIPStartFlag`
*	:ref:`option-GUROBI-mip_start` 
