.. _GUROBI_Presolve_-_Presolve_Aggregation_Fill:


Presolve Aggregation Fill
=========================



**Type**:	Integer	

**Range**:	{-1 .. 2000000000}	

**Default**:	-1	



This option controls the amount of fill allowed during presolve aggregation. Larger values generally lead to presolved models with fewer rows and columns, but with more constraint matrix non-zeros. The default value of -1 chooses automatically.



