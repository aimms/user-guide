.. _option-ODHCPLEX-primal_pricing_algorithm:


Primal Pricing Algorithm
========================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Hybrid + Devex	



This option can be used to select the pricing algorithm for the primal simplex method. While the default pricing usually provides the fastest solution time, problems may benefit from alternate settings. Possible values are:



    *	Reduced Cost (reduced-cost pricing)
    *	Hybrid + Devex (hybrid reduced-cost and Devex pricing)
    *	Devex (Devex pricing)
    *	Steepest edge (steepest-edge pricing)
    *	Steepest edge + slack norms (steepest-edge pricing with slack initial norms)
    *	Full pricing



