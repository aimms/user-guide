

.. _XA_Troubleshooting:


Troubleshooting
===============

**Out of memory** 

When trying to solve a large model, XA might sometimes fail to load the model and return the message "Memory allocation error; requested memory not available." followed by the message "XA tried to allocate x Mb of memory to load the model and failed.".



XA uses a formula to calculate the amount of memory that XA expects it needs for loading a model. (This formula is based on the number of rows, columns and nonzero matrix elements.) For some models this formula is not very accurate and its outcome might be too high; sometimes higher than the amount of memory available to XA. In this situation you can use the general solvers option **Solver Workspace**  to set the amount of memory XA should use (XA will then not use the formula). The value of the option **Solver Workspace**  should be set to a value smaller than the x in the message "XA tried to allocate x Mb of memory to load the model and failed." (and it should be higher than 0).



It can also happen that the amount of memory calculated with the formula is accurate and that there is not enough memory available to load the model in XA. If you are using a 32 bits version of AIMMS then you should consider using a 64 bits version.



**Learn more about** 

*	:ref:`Options_Memory_-_Solver_Workspace` 






