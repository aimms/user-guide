.. _option-KNITRO-act_qppenalty:


Act QPpenalty
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic



This option indicates whether to use a penalty formulation for quadratic programming (QP) subproblems in the Knitro SQP algorithm, which offers improved performance. At the default setting Knitro will automatically decide whether to penalize constraints in QP subproblems. Possible values are:



    *	Automatic
    *	No penalized constraints
    *	Penalize all constraints

	







