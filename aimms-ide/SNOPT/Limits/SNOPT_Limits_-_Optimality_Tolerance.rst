.. _SNOPT_Limits_-_Optimality_Tolerance:


Optimality Tolerance
====================



**Type**:	Floating point number	

**Range**:	[0,1000]	

**Default**:	1e-6	



This option is used to judge the optimality for each QP subproblem.



Let the QP reduced gradient be dj = gj - pTaj, where gj is the jth component of the QP gradient, aj is the associated column of the QP matrix, and p is the set of QP dual variables.



By construction, the reduced gradients for basic variables are always zero. The QP subproblem will be declared optimal if the reduced gradients for nonbasic variables at their lower or upper bounds satisfy



dj ``/ ||`` p``|| >= - t`` or  dj ``/ ||`` p``|| <= t`` ``,`` 



repectively, and if dj``/ ||`` p``|| <= t`` for superbasic variables (where t denotes the optimality tolerance).



In the above tests, ``||`` p``||``  is a measure of the size of the dual variables. It is included to make the tests independent of a large scale factor on the objective function. The quantity actually used is defined by



``||`` p `` || =`` max{ d / Öm, 1 },  where  :math:`d = åi  | pi |`.



If the objective is scaled down to be very small, the optimality test reduces to comparing dj against t.



**Learn more about** 

*	:ref:`SNOPT_Limits_-_Major_Optimality_Tole`  



