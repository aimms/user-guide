

.. _option-AIMMS-warning_unused_index:


Warning Unused Index
====================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default		



This option determines what happens during compilation when an index of an iterative operator is not used
in the expressions inside that iterative operator. In addition, it warns against the use of an index in the
index domain of a constraint that is not used in the definition of that constraint.

Consider the example:

.. code-block:: aimms

    a(i) := sum( (j,k), b(i,j) );


In this example the result of ``sum( (j,k), b(i,j) )`` does not depend on ``k``, and this assignment could
thus be rewritten more efficiently as:

.. code-block:: aimms

    a(i) := Card(Set_K) * sum( j, b(i,j) );

In addition, consider the following example:

.. code-block:: aimms

    Constraint limX {
        IndexDomain: (i,j) | C(i,j);
        Definition: sum( k, x(i,k) ) <= r(i);
    }


In this example, the index ``j`` is not used in the definition of constraint ``limX`` and thus leads to
the generation of duplicate rows. The above constraint can be rewritten as follows, avoiding duplicate rows:

.. code-block:: aimms

    Constraint limX {
        IndexDomain: (i) | exists( j | C(i,j) );
        Definition: sum( k, x(i,k) ) <= r(i);
    }


An unused index situation will be ignored, reported as a warning, or interpreted as an error, depending on the following settings:


.. list-table::

   * - *	Off	
     - Do not issue a warning.
   * - *	Warning_collect
     - Issue a warning and post it to the global error and warning collector.
   * - *	Common_warning_default
     - Take action depending on the option 'Common warning default'.
   * - *	Warning_handle
     - Issue a warning and post it to the nearest error handler.
   * - *	Strict_warning_default
     - Take action depending on the option 'Strict warning default'.
   * - *	Error
     - Issue an error.
   * - *	Error_in_develop_else_warning
     - In a developer system same as Error, in a deployment system same as Warning_handle
   * - *	Error_in_develop_else_off
     - In a developer system same as Error, in a deployment system same as Off
   * - *	Warning_in_develop_else_off
     - In a developer system same as Warning_handle, in a deployment system same as Off


**Note** 

*	With the option **Maximal Number of Warnings Reported** you can set the maximal number of warnings that are shown in errors/warnings and message window.


**Learn more about** 

*	:ref:`option-AIMMS-maximal_number_of_warnings_reported` 
*	:ref:`option-AIMMS-common_warning_default` 
*	:ref:`option-AIMMS-strict_warning_default` 
*	:ref:`option-AIMMS-communicate_warnings_to_end_users` 

