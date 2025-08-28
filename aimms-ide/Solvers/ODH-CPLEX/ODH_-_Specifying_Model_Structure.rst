.. _ODH-CPLEX_-_Specifying_Model_Structure:


Specifying Model Structure
==========================

**Description** 

ODH-CPLEX needs to break the specified matrix down into sub-models. It can do this in one of two ways:




*   Automatically using its decomposition heuristic; or
*   By assigning each variable to a different block (or ‘key’).



You can specify a decomposition yourself by assigning a variable to a different block using the routine GMP::Column::SetDecomposition. By default, the program will use information specified by the user through this routine, and its automatic decomposition heuristic otherwise.



The automatic decomposition heuristic divides the model up into parts, using an **Initial Divisor Value**. Initially this is a number not less than 2 and it is increased as the search progresses. When no improved solution is found after a number, **Maximum Divisor Repeats**, of attempts with the maximum interval divisor, **Maximum Divisor Value**, the program terminates. Default values are provided for **Maximum Divisor Repeats**  and **Maximum Divisor Value**, so these do not have to be specified by the user.



Whilst the automatic decomposition method often works well, there may be an advantage to specifying decomposition through the routine GMP::Column::SetDecomposition. After performing the decomposition in whatever way, the program analyses the decomposition and displays statistics showing the maximum and minimum number of variables in each key or block and showing a percentage score to the decomposition as a whole. A typical display is of the form:



Variables/key 205.58 (+/-304.79), max/min variables/key 933(32) / 60(113).

There are 227 keys (4149 keys were dropped) with 46872 values.      

Decomposition score 13.66%, graph score 2074/3135232.           



Other things (such as the distribution of variables in keys and the number of keys) being equal, the smaller the percentage decomposition score, the better the decomposition is and the more effective the program will be.



**Learn more about** 

*	:ref:`option-ODHCPLEX-initial_divisor_value`  
*	:ref:`option-ODHCPLEX-maximum_divisor_repeats`  
*	:ref:`option-ODHCPLEX-maximum_divisor_value`  
*	:any:`GMP::Column::SetDecomposition`
