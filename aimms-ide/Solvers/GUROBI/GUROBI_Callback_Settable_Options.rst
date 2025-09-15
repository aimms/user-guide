
.. _GUROBI_Callback_Settable_Options:


Callback Settable Options
=========================

A few options that control the termination of the solving process can be modified from within a callback within Gurobi (version 12.0
or higher), using the procedure :any:`GMP::SolverSession::SetOptionValue`. These options are:

    -	:ref:`option-AIMMS-time_limit`
    -	:ref:`option-GUROBI-barrier_iteration_limit`
    -	:ref:`option-GUROBI-feasibility_pump_passes`
    -	:ref:`option-GUROBI-node_limit`
    -	:ref:`option-GUROBI-work_limit`


This makes it easier to implement custom termination criteria that, for example, set a time limit based on dynamic solving process data
like the current MIP gap. For example:

.. code-block:: aimms

   Procedure IncumbentCallback {
       Arguments: (ThisSession);
       Body: {
           Obj := GMP::SolverSession::GetObjective( ThisSession );
           BestBound := GMP::SolverSession::GetBestBound( ThisSession );
           MIPgap := abs( (Obj - BestBound) / Obj );
           
           if ( MIPgap <= 0.05 ) then
               GMP::SolverSession::SetOptionValue( ThisSession, "Time limit", 60 );
           endif;
           
           return 1;
       }
       ElementParameter ThisSession {
           Range: AllSolverSessions;
           Property: Input;
       }
       Parameter Obj;
       Parameter BestBound;
       Parameter MIPgap;
   }

In this example the time limit is set to 60 seconds once the MIP gap reaches 5%.


**Note** 

*	The constraint must be linear; a quadratic constraint is not allowed to be an indicator constraint.

