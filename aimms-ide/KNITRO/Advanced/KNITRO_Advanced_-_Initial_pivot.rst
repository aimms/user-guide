.. _KNITRO_Advanced_-_Initial_pivot:


Initial Pivot Treshold
======================



**Type** :	Floating point number	

**Range** :	[0,0.5]	

**Default** :	1e-8	



This option specifies the initial pivot threshold used in the factorization routine. Higher values for this option result in more pivoting (more stable factorization). If the value equals 0 then no pivoting will be performed. Smaller values may improve the speed of the code but higher values are recommended for more stability (for example, if the problem appears to be very ill-conditioned).





