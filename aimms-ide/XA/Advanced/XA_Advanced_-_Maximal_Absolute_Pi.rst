.. _option-XA-maximal_absolute_pivot_value:


Maximal Absolute Pivot Value
============================



:Type:	Real	
:Range:	[0,1]	
:Default:	1e-6	



After a column is selected to enter the basis, a column is selected to leave the basis to keep the model feasible. When selecting a column to leave the basis only columns are considered that have a marginal value that is greater than the value of option **Minimal Absolute Pivot Value**  (in absolute sense). Among these columns a column is chosen which has a marginal value that is greater than the value of this option (in absolute sense). When no such column exists XA searches for another column to enter the basis, and the search for a leaving column is performed again until a column is found with a marginal value greater than the value of this option (in absolute sense). If all entering columns are rejected XA selects the entering column with the largest marginal value.



**Remark** 

Extreme caution should be exercised when changing the value of this option because of the overall effect on problem feasibility.



**Learn more about** 

*	:ref:`option-XA-minimal_absolute_pivot_value`  



