

.. _option-IPOPT-constraint_multipliers_initial_guess_limit:


Constraint Multipliers Initial Guess Limit
==========================================



:Type:	Floating point number	
:Range:	[0,1e+019]	
:Default:	1000	



This option determines how large the initial least-square guesses of the constraint multipliers are allowed to be (in max-norm). If the guess is larger than this value, it is discarded and all constraint multipliers are set to zero. This option is also used when initializing the restoration phase.

