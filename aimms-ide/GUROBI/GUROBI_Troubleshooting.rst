.. _GUROBI_Troubleshooting:


Troubleshooting
===============

**Could not initialize DLL libgrb120.dll** 

You can get this error if you use a 'link-only' licence for Gurobi. To resolve this do the following steps:



*	Have the Gurobi license installed correctly; you should be able to run Gurobi stand-alone.
*	Set the (Windows) environment variable GRB_LICENSE_FILE to point to the exact location of the license file. For example, if the license file gurobi.lic is in the directory C:\Gurobi, then set GRB_LICENSE_FILE to C:\Gurobi\gurobi.lic. (Please note that you should restart AIMMS if you set or change the environment variable GRB_LICENSE_FILE while AIMMS is open.)




**Out of memory** 


If Gurobi fails to do a postsolve due to insufficient memory available (while there was enough memory available to do the normal solve) then you might consider to turn off the postsolve by switching off the general solvers option **Postsolve** .





**Presolver declares model infeasible** 


In case the Gurobi Presolver declares a model as infeasible, the solution reported by Gurobi can usually not be used to analyse where your problem formulation proved infeasible. To get a solution that can be interpreted, you have to rerun your model with the option **Presolve**  turned off.





**Learn more about** 

*	:ref:`Options_Postsolve_-_Postsolve` 
*	:ref:`option-GUROBI-presolve`  



