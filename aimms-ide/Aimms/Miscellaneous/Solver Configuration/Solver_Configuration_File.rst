

.. _Miscellaneous_Solver_Configuration_File:


Solver Configuration File
=========================

**Description** 

The information displayed in the Solver Configuration dialog box is read from and written to the solver configuration file. If no solver configuration file exists then AIMMS will create (at startup) a standard solver configuration file based on the AIMMS license and the available solvers in the AIMMS installation. The solver configuration file is editable and has the following layout:



! Format AIMMS380

! solver name   / dll name       / model types for which solver is the default

AOA        / libaoa.dll      / MIQP MIQCP MINLP

CONOPT 4.0    / libconopt40.dll    / NLP QCP

XA 16       / libxa16.dll      / LP MIP QP



The first column contains the solver name as it will be used inside AIMMS. The second column contains the name of the AIMMS-solver interface dll inside the Solvers directory of the AIMMS installation. The last column contains the model types for which the solver is the default solver.



Lines with a '!' in front are treated as comment. The first line is required otherwise AIMMS will not recognize it is a solver configuration file that uses the 380 format. Old solver configuration files are automatically converted to the new format.



AIMMS keeps its solver configuration file (with extension .slv) in the folder AIMMS of the common application area of your computer. It is possible to place a solver configuration file in the project directory which then must have the name 'solvers.slv'. In that case AIMMS will use that file for reading and writing, and ignore the general solver configuration file. In this way it is possible to use a project dependent solver configuration.



You can create a solver configuration file in the project directory by clicking the Export button in the Solver Configuration dialog box.



If AIMMS cannot find a solver then it will try to find another version of that solver, and in case of success, AIMMS will add the solver version to the solver configuration file. AIMMS will also automatically update the solver configuration file if it finds a newer version of a solver (but it will not be made the default) or if one of the model types is missing. However, a project dependent solver configuration file, as described above, will never be automatically updated.



If the AIMMS license is upgraded to include more solvers then AIMMS will update the solver configuration the first time AIMMS is started after the license upgrade; the latest version of those solvers will then be added.



**Note** 

*	If the solver configuration file contains a solver that is not licensed then AIMMS will generate an error at startup. You can circumvent this in a project dependent solver configuration file by adding a '*' at the end of a line with a solver, in which case the solver will be skipped.




**Learn more about** 

*	:ref:`Miscellaneous_Solver_Configuration`  



