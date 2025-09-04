

.. _option-AIMMS-warning_variable_suffix_ambiguity:


Warning Variable Suffix Ambiguity
=================================



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Common_warning_default		



This option determines what happens during the compilation of the definition attribute of a constraint,
when a variable is used as argument of a function where a parameter is expected.

Consider the example:

.. code-block:: aimms

    Set myBSet {
        Index: b;
    }
    Set myOSet {
        Index: o;
    }
    Variable X {
        IndexDomain: b;
        Range: binary;
    }
    ElementVariable Y {
        IndexDomain: o;
        Range: myBSet;
    }
    Variable Z {
        IndexDomain: o;
        Range: {0 .. 10};
    }
    Constraint eqn {
        IndexDomain: (i,j) | C(i,j);
        Definition: cp::BinPacking( b, X(b), o, Y(o), Z(o) );
    }


Here, in the fifth argument of :any:`cp::BinPacking`, the weights are supposed to be entered as a parameter.
Thus AIMMS will issue the following warning message:

.. code-block:: text

    Warning: Variables are allowed in constraint definitions, but not at the fifth argument of "cp::BinPacking".
    The current level value of variable "Z" is used instead, as if this variable is a parameter. If you intended
    to use this variable as a variable, you will have to rewrite the constraint. If you intended to use the current
    level value of this variable, you will have to use the suffix .Level explicitly in order to suppress this warning.


A variable used as argument of a function where a parameter is expected while compiling the definition of a constraint,
will be ignored, reported as a warning, or interpreted as an error, depending on the following settings:


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

