

.. _Options_NonlinPres_-_RemoveDoubletons:


Remove Doubletons
=================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Automatic	



This option controls whether the AIMMS Presolver should remove so called doubletons. Possible values are:



*	Never
*	Automatic
*	Always




A doubleton is defined by two variables that appear in a constraint of the form X = aY, where X and Y are two variables and a is a value unequal to 0. If such a doubleton exists then X can be replaced by aY in all constraints, and variable X and the constraint X = aY can be deleted.





If the value equals 'Automatic' then the AIMMS Presolver will remove all doubletons if the model is linear. For a nonlinear model, doubletons will be removed if the level values of the two variables match. For example, if X = 3Y then this doubleton will only be removed if the level value of X equals three times the level value of Y. This option setting is useful for nonlinear models in which the user has specified initial level values for the variables. With this setting the AIMMS Presolver chooses to use the initial level values of both variables instead of removing the doubleton, in case the level values do not match.





If the value of this option is 'Always' then the AIMMS Presolver will remove all doubletons.





**Note** 

*	This option has only an effect when solving a nonlinear model and the option **Nonlinear Presolve**  is switched on, or when solving a linear, quadratic or quadratically-constrained model and the option **Linear Presolve**  is switched on, or if the function GMP::Instance::CreatePresolved is used.




**Learn more about** 

*	:ref:`Options_NonlinPres_-_LinearPresolve` 
*	:ref:`Options_NonlinPres_-_NonlinearPresolve`  



