.. _option-KNITRO-mip_heuristic:


MIP Heuristic
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option specifies which MIP heuristic search approach to apply to try to find an initial integer feasible point. Possible values are:



    *	Automatic
    *	None
    *	Not used
    *	Feasibility pump
    *	MPEC
    *	Diving




Setting 'None' disables heuristic search. Setting 'MPEC' implies that the heuristic is applied based on the MPEC formulation.





If a heuristic search procedure is enabled, the maximum number of iterations before starting the branch and bound procedure is specified by the option **MIP Heuristic Iteration Limit** .





Note: This option has been deprecated since Knitro version 12.4. As alternatives, you can use :ref:`option-KNITRO-mip_heuristic_diving` , :ref:`option-KNITRO-mip_heuristic_feasibility_pump` , :ref:`option-KNITRO-mip_heuristic_mpec` , and :ref:`option-KNITRO-mip_heuristic_strategy` .





**Learn more about** 

*	:ref:`option-KNITRO-mip_heuristic_diving` 
*	:ref:`option-KNITRO-mip_heuristic_feasibility_pump` 
*	:ref:`option-KNITRO-mip_heuristic_mpec` 
*	:ref:`option-KNITRO-mip_heuristic_strategy` 
