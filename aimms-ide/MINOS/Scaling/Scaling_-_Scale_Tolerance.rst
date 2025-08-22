

.. _option-MINOS-scale_tolerance:


Scale Tolerance
===============



:Type:	Floating point number	
:Range:	[0.0001, 0.9999]	
:Default:	0.9	



This option affects how many passes might be needed through the constraint matrix. On each pass, the scaling procedure computes the ratio of the largest and smallest nonzero coefficients in each column. If this ratio is smaller than r times (r denoting the scale tolerance) its previous value, another scaling pass is performed to adjust the row and column scales. Raising r from 0.9 (the default) to 0.99 (say) usually increases the number of scaling passes through A. At most 10 passes will be made.



