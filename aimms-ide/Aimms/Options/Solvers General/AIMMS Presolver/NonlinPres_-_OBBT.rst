

.. _Options_NonlinPres_-_OBBT:


OBBT
====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option controls whether the AIMMS Presolver will apply Optimization-Based Bound Tightening (OBBT). Possible values are:



*	Off
*	Automatic
*	Full




During OBBT up to 2n LP problems will be solved to find tighter upper and lower bounds for the variables. Here n denotes the number of variables. Because this can be a time-consuming step, OBBT is switched off by default.





OBBT is applied after the AIMMS Presolver has done one iteration of the Feasibility-Based Bound Tightening (FBBT) algorithm for reducing variable bounds. At the 'Automatic' setting, OBBT will only be applied to variable bounds that were not tightened after using (one iteration of) FBBT. At the 'Full' setting, OBBT will be applied to all variable bounds.





**References** 

*	Belotti, P., J. Lee, L. Liberti, F. Margot, A. Wächter, Branching and bounds tightening techniques for non-convex MINLP. Optimization Methods & Software **24**  (2009), pp. 597-634.



