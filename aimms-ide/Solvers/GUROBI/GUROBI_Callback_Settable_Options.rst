
.. _GUROBI_Callback_Settable_Options:


Callback Settable Options
=========================

A few options that control the termination of the solving process can be modified from within a callback within Gurobi (version 12.0
or higher), using the procedure :any:`GMP::SolverSession::SetOptionValue`. These options are:

    -	:doc:`Stop_Criteria_-_Time_Limit <../../Aimms/Options/Solvers General/Stop Criteria/Stop_Criteria_-_Time_Limit>`
    -	:doc:`GUROBI_Barrier_-_Barrier_Iteration_Limit <Barrier/GUROBI_Barrier_-_Barrier_Iteration_Limit>`
    -	:doc:`GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes <MIP Heuristics/GUROBI_MIP_Heuristic_-_Feasibility_Pump_Passes>`
    -	:doc:`GUROBI_MIP_-_Node_Limit <MIP/GUROBI_MIP_-_Node_Limit>`
    -	:doc:`GUROBI_General_-_Work_Limit <General/GUROBI_General_-_Work_Limit>`


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

