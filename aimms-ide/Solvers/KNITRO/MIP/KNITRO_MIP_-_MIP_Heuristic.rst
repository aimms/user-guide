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





If a heuristic search procedure is enabled, the maximum number of iterations before starting the branch and bound procedure is specified by the option **MIP Heuristic Iteration Limit**.





Note: This option has been deprecated since Knitro version 12.4. As alternatives, you can use :doc:`KNITRO_MIP_-_MIP_Heuristic_Diving <KNITRO_MIP_-_MIP_Heuristic_Diving>` , :doc:`KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump <KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump>` , :doc:`KNITRO_MIP_-_MIP_Heuristic_MPEC <KNITRO_MIP_-_MIP_Heuristic_MPEC>` , and :doc:`KNITRO_MIP_-_MIP_Heuristic_Strategy <KNITRO_MIP_-_MIP_Heuristic_Strategy>` .





**Learn more about** 

*	:doc:`KNITRO_MIP_-_MIP_Heuristic_Diving <KNITRO_MIP_-_MIP_Heuristic_Diving>` 
*	:doc:`KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump <KNITRO_MIP_-_MIP_Heuristic_Feasibility_Pump>` 
*	:doc:`KNITRO_MIP_-_MIP_Heuristic_MPEC <KNITRO_MIP_-_MIP_Heuristic_MPEC>` 
*	:doc:`KNITRO_MIP_-_MIP_Heuristic_Strategy <KNITRO_MIP_-_MIP_Heuristic_Strategy>` 
