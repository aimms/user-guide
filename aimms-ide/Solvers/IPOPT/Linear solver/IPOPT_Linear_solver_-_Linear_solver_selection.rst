

.. _option-IPOPT-linear_solver_selection:


Linear solver selection
=======================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	MUMPS solver	



This option determines which linear algebra package is to be used for the solution of the augmented linear system (for obtaining the search directions). It is important to keep in mind that usually the largest fraction of computation time in the optimizer is spent for solving the linear system, and that the choice of the linear solver impacts IPOPT's speed and robustness. Possible values are:



    *	MUMPS solver
    *	HSL routine MA27
    *	HSL routine MA57
    *	HSL_MA77
    *	HSL_MA86
    *	HSL_MA97
    *	Pardiso solver




By default, IPOPT in AIMMS only supports the public domain solver MUMPS. Some publications on MUMPS are:





P. R. Amestoy, I. S. Duff, J. Koster and J.-Y. L'Excellent, **A fully asynchronous multifrontal solver using distributed dynamic scheduling**, SIAM Journal of Matrix Analysis and Applications, Vol 23, No 1, pp 15-41 (2001). 





P. R. Amestoy and A. Guermouche and J.-Y. L'Excellent and S. Pralet, **Hybrid scheduling for the parallel solution of linear systems**, Parallel Computing, Vol 32 (2), pp 136-156 (2006). 





Using the "library loader", a Pardiso DLL or a DLL with HSL (Harwell Subroutine Library) subroutines (which the user has to compile) can be loaded at runtime. The third party software for Pardiso and HSL is released under different licenses than IPOPT. For this reason that code is not distributed together with the IPOPT package and therefore you have to go through the hassle of obtaining it yourself.





The Pardiso DLL or HSL DLL should be placed in the Solvers directory of the AIMMS installation. Alternatively, you can also place the DLL into a directory which is added to the PATH environment variable on Windows or to the LD_LIBRARY_PATH search path on Linux.





Instructions for building the HSL DLL can be found in the section :ref:`HSL_libraries`. 
Information about the recommended HSL solver can be found in the `HSL for IPOPT <https://licences.stfc.ac.uk/product/coin-hsl>`_ link.





See the prerequisites for IPOPT for more information on these third party components. Keep in mind that it is YOUR RESPONSIBILITY to ensure that your downloading and usage of the third party components conforms with their licenses.





**Learn more about** 

*	:ref:`HSL_libraries` 
*	`IPOPT: Prerequisites <https://coin-or.github.io/Ipopt/INSTALL.html>`_ (Internet link)
*	`MUMPS <https://mumps-solver.org>`_ (Internet link)
*	`HSL for IPOPT <https://licences.stfc.ac.uk/product/coin-hsl>`_ (Internet link)
*	`Pardiso <https://panua.ch/products/pardiso/>`_ (Internet link)
