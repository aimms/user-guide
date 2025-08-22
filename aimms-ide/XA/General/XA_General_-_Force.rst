.. _option-XA-force:


Force
=====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	No	



This option can be used to find the Irreducible Infeasible Subsets (IISs) of an infeasible LP model. If force equals 'Yes' then the model is internally modified prior to solving, such that, if the model is infeasible XA will isolate Irreducible Infeasible Subsets of constraints.



Only run with force equal to 'Yes' to get Irreducible Infeasible Subsets as it turns the presolver off, consumes significant amounts of memory, and solves much slower. 



Possible values are:



*	No
*	Yes







**Remark** 


To find Irreducible Infeasible Subsets with XA also the global solvers option **Infeasibility Finder**  should be switched on.





**Learn more about** 

*		:ref:`option-AIMMS-infeasibility_finder`  



