

.. _HSL_libraries:
.. _IPOPT_HSL_libraries:


HSL libraries
=============

By default, IPOPT in AIMMS only supports the public domain solver MUMPS as linear algebra package for the solution of the augmented linear system (for obtaining the search directions). It is important to keep in mind that usually the largest fraction of computation time in the optimizer is spent for solving the linear system.



Using the "library loader", a DLL with HSL (Harwell Subroutine Library) subroutines (which the user has to compile) can be loaded at runtime. The third party software for HSL is released under different licenses than IPOPT. For this reason that code is not distributed together with the IPOPT package and therefore you have to go through the hassle of obtaining it yourself.



See the prerequisites for IPOPT for more information on these third party components. Keep in mind that it is YOUR RESPONSIBILITY to ensure that your downloading and usage of the third party components conforms with their licenses.



Information about the recommended HSL solver can be found in the `HSL for IPOPT <https://licences.stfc.ac.uk/product/coin-hsl>`_ link.



**Instructions for HSL using MS Visual Studio Fortran** 

To use a HSL routine for the Linear Solver Selection the user has to do the following. For HSL with MA57 the instructions are:



1.	Download, e.g., Ipopt-3.11.0.zip from `http://www.coin-or.org/download/source/Ipopt/ <https://www.coin-or.org/download/source/Ipopt/>`_ and unzip the file.

2.	The file Ipopt-3.11.0\Ipopt\MSVisualStudio\v8-ifort\libhsl\libhsl.vfproj (can be opened using a normal editor) shows which HSL .f files are needed if MA57 is used. 

3.	Obtain the HSL Fortran files from `http://www.hsl.rl.ac.uk/ <https://www.hsl.rl.ac.uk/>`_ and place them in directory Ipopt-3.11.0\ThirdParty\HSL. 

4.	Open IpOpt-ifort.sln in Ipopt-3.11.0\Ipopt\MSVisualStudio\v8-ifort using MS Visual Studio Fortran.

5.	Build the libhsl project. 

6.	Copy the resulting libhsl.dll to the Solvers directory of AIMMS. Alternatively, you can also place libhsl.dll into a directory which is added to the PATH environment variable on Windows or to the LD_LIBRARY_PATH search path on Linux.



For HSL without MA57 the instructions for step 2 and 5 are slightly different:



2a.	The file Ipopt-3.11.0\Ipopt\MSVisualStudio\v8-ifort\libhsl-no-MA57\libhsl-no-MA57.vfproj (can be opened using a normal editor) shows which HSL .f files are needed if MA57 is not used. 

5a.	Build the libhsl-no-MA57 project.



After building libhsl.dll and copying it, you can select HSL as the linear solver by using the option **Linear Solver Selection** .



**Learn more about** 

*	:ref:`IPOPT_Linear_solver_-_Linear_solver_selection` 
*	`HSL for IPOPT <https://licences.stfc.ac.uk/product/coin-hsl>`_ (Internet link)
