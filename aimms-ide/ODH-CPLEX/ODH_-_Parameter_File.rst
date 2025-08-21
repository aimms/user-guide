.. _ODH-CPLEX_-_Parameter_File:

Parameter File
==============

**Description** 

You can use a parameter file to specify ODH-CPLEX options. 
Options that influence the heuristic sub-model CPLEX solves or the heuristic sub-model CPLEX solves in Phase I, 
this is the only way to set these options. 
The parameter file should be named 'odh.prm' and should be placed in the main AIMMS project folder 
(i.e., the folder containing the .aimms file). 
If the parameter file is present then it will be used by ODH-CPLEX.

The ODH-CPLEX parameter name corresponding to an AIMMS option can be found in :ref:`AIMMS_to_ODH_Mapping`. 
The syntax for the parameters that influence the heuristic sub-model CPLEX solves is the following: SUB_<parameter> 
where <parameter> refers to the ODH-CPLEX parameter name (for the main CPLEX solve in ODH-CPLEX). 
The syntax for the parameters that influence the heuristic sub-model CPLEX solves in Phase I is the following: PHASE1_<parameter>. 
For example, SUB_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model, 
while PHASE1_CPX_RINSHEUR specifies the RINS heuristic frequency for CPLEX if it used to solve a heuristic sub-model in Phase I.

The content of the parameter file could be:

.. code-block:: none

    THREADS = 4     
    CPX_RINSHEUR = 5   
    SUB_CPX_RINSHEUR = 5 

The first line sets the**Thread Limit**  (which is an ODH engine option) to 4. 
The second line sets the **RINS Heuristic Frequency**  to 5 for the main CPLEX solve in ODH-CPLEX while 
the third line sets it to 5 for the heuristic sub-model CPLEX solves.

**Learn more about** 

*   :ref:`AIMMS_to_ODH_Mapping`  
*   :ref:`option-ODHCPLEX-rins_heuristic_frequency`  
*   :ref:`option-ODHCPLEX-thread_limit`  



