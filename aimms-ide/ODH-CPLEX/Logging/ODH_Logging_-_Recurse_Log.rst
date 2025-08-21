.. _option-ODHCPLEX-recurse_log:


Recurse Log
===========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to write thread log files for the recurse heuristic for sub-solves. Possible values are:



*	No
*	Yes




The log files are named 'odh.x.rec.log' where x is the number of the thread (starting at 0), and these files are placed in the main project folder.





This option is only active if the option **Recurse**  is set to a value other than 'Off'.





**Learn more about** 

*	:ref:`option-ODHCPLEX-recurse`  
