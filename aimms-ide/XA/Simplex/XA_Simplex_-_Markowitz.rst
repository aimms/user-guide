.. _XA_Simplex_-_Markowitz:


Markowitz
=========



:Type:	Real	
:Range:	[0,1e+023]	
:Default:	10.0	



The setting of this option is used during matrix inversion and updating of the LU factors. During inversion, rows and columns are scanned for the largest and smallest numbers (in absolute sense). The pivot element is chosen such that the ratio of the pivot element to these numbers is less than the value of this option if possible. The larger this value is, the larger will be this ratio, which can cause numeric instability. The best number for numeric stability is 1.0, which tends to lead to fill-in the LU factors and reduced speed.



In summary: a value of 1.0 is the best for numerical stability and the worst for fill-in, whereas a value of 1000.0 is (can be) bad for numerical stability but good to maintain sparsity of LU factors.



