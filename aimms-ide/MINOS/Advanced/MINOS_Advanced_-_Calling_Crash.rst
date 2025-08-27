.. _option-MINOS-calling_crash_procedure:


Calling Crash Procedure
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Call Crash three times	



Except on restarts, a Crash procedure is used to select an initial basis from certain rows and columns of the constraint matrix :math:`(A - I)`.
This option determines which rows and columns of :math:`A` are eligible initially, and how many time Crash is called. Columns
of :math:`- I` are used to pad the basis where necessary.



With the setting 'Choose all-slack basis B = I' the initial basis contains only slack variables (i.e., :math:`B = I`). When the value of
this option equals 'Call Crash once' Crash is called once, looking for a triangular basis in linear rows. If it equals 'Call Crash twice',
Crash is called twice if there are nonlinear constraints. The first call looks for a triangular basis in linear rows, and the
iteration proceeds with simplex iterations until the linear constraints are satisfied. The Jacobian is then evaluated for the first
major iteration and Crash is called again to find a triangular basis in the nonlinear rows (retaining the current basis for linear rows).
If the value of this option equals 'Call Crash three times' (the default) Crash is called first twice to treat linear equalities and
linear inequalities separately. The last call treats nonlinear rows before the first major iteration (as for 'Call Crash twice').



If the setting 'Choose all-slack basis B = I' is not selected, certain slacks on inequality rows are selected for the basis first.
(If Crash is called twice or three times, numerical values are used to exclude slacks that are close to a bound.) Crash then makes
several passes through the columns of :math:`A`, searching for a basis matrix that is essentially triangular. A column is assigned to "pivot"
on a particular row if the column contains a suitably large element in a row that has not yet been assigned. (The pivot elements
ultimately form the diagonals of the triangular basis.) For remaining unassigned rows, slack variables are inserted to complete the basis.



Possible values are:



*	Choose all-slack basis B = I
*	Call Crash once
*	Call Crash twice
*	Call Crash three times




**Learn more about** 

*	:ref:`option-MINOS-crash_tolerance`  






