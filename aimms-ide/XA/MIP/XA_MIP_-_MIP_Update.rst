.. _XA_MIP_-_MIP_Update:


MIP Update
==========



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Yes	



When solving an updated version of an already loaded model, XA retrieves these updates from AIMMS, modifies the model and solves the model using the results of the previous solve. This means that the basis present in XA is used. Although such a basis can provide a good starting point, it does not always have to be in case of an updated MIP model. It may even be better to reload the updated model with the option **MIP Basis**  set to no, in order to gain performance enhancements as a result of presolving and crashing the updated MIP model. If you want to solve each MIP afresh, then set both this option and the option **MIP Basis**  to no. Possible values are:



*	No
*	Yes




**Learn more about** 

*	:ref:`XA_MIP_-_MIP_Basis`  



