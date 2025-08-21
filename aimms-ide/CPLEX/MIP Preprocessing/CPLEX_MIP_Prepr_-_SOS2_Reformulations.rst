.. _option-CPLEX-sos2_reformulations:


SOS2 Reformulations
===================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option allows you to control the reformulation of special ordered sets of type 2 (SOS2), which can be applied during the solution process of problems containing these sets. Possible values are:



*	Off
*	Automatic
*	On




Setting the value of this parameter to 'Automatic', the default, specifies that the SOS2 should be reformulated as linear constraints only if this is deemed to be helpful.





A special ordered set (SOS) can be used for modeling complex nonlinearities, for example, disjunctive constraints or piecewise linear functions, in an easy and natural way. However, in order to achieve good performance and effectively solve the problem, during the solution process it can be advantageous to reformulate the special ordered sets as linear constraints, by introducing additional variables into the problem formulation.





CPLEX implements a logarithmic reformulation of special ordered sets, where each SOS is reformulated by adding to the problem a number of binary variables and extra linear constraints which are logarithmic in the size of the SOS. By default, CPLEX automatically decides whether a SOS should be reformulated or not.





For a more thorough exploration of the theory supporting SOS reformulations, see, for example, the reference below.





**References** 

*	J.P. Vielma, J.P., G.L. Nemhauser, Modeling disjunctive constraints with a logarithmic number of binary variables and constraints. Mathematical Programming **128**  (2011), pp. 49-72.




**Learn more about** 

*	:ref:`option-CPLEX-sos1_reformulations`  
