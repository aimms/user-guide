.. _option-XA-perturbate:


Perturbate
==========



:Type:	Real	
:Range:	[0,1]	
:Default:	0.0	



XA counts the number of degenerate iterations (pivots) that are performed. If this number equals the value of the option **Degenerate Pivots** , zero pivot values are adjusted by the value of this option in an attempt to move away from this region. After a non-degenerate pivot is made the counter for the number of degenerate pivots is reset to zero.



**Remark** 

Extreme caution should be exercised when changing the value of this option because of the overall effect on problem feasibility.



**Learn more about** 

*	:ref:`option-XA-degenerate_pivots`  



