
PATH
====

**Description** 

PATH is a tool for solving (square) mixed complementarity problems. Mixed complementarity problems are systems of linear and nonlinear constraints
where variables in the model are linked to constraints in the form of mixed complementarity conditions. In AIMMS, a mixed complementarity
condition is defined as follows for a given variable :math:`x_i` and an associated function :math:`f_i(x)`.

If :math:`l_{if} = -\infty` and :math:`u_{if} = \infty` then

.. list-table::

   * - either
     - :math:`x_i = l_{ix}`
     - and
     - :math:`f_i(x) \geq 0`
   * - or
     - :math:`x_i = u_{ix}`
     - and
     - :math:`f_i(x) \leq 0`
   * - or
     - :math:`l_{ix} < x_i < u_{ix}`
     - and
     - :math:`f_i(x) = 0`.


If :math:`l_{ix} = -\infty` and :math:`u_{ix} = \infty` then

.. list-table::

   * - either
     - :math:`x_i = 0`
     - and
     - :math:`l_{if} < f_i(x) < u_{if}`
   * - or
     - :math:`x_i \geq 0`
     - and
     - :math:`f_i(x) = l_{if}`
   * - or
     - :math:`x_i \leq 0`
     - and
     - :math:`f_i(x) = u_{if}`


In any other situation, where *exactly* two of the constants :math:`l_{ix}`, :math:`u_{ix}`, :math:`l_{if}` and :math:`u_{if}` are finite, then

.. list-table::

   * - either
     - :math:`x_i = l_{ix}`
     - and
     - :math:`l_{if} \leq f_i(x) \leq u_{if}`
   * - or
     - :math:`x_i = u_{ix}`
     - and
     - :math:`l_{if} \leq f_i(x) \leq u_{if}`
   * - or
     - :math:`l_{ix} < x_i < u_{ix}`
     - and
     - :math:`f_i(x) = l_{if}`
   * - or
     - :math:`l_{ix} < x_i < u_{ix}`
     - and
     - :math:`f_i(x) = u_{if}`


**Transformation** 

PATH uses a different definition. In PATH, a mixed complementarity condition requires that:

.. list-table::

   * - either
     - :math:`x_i = l_{ix}`
     - and
     - :math:`f_i(x) \geq 0`
   * - or
     - :math:`x_i = u_{ix}`
     - and
     - :math:`f_i(x) \leq 0`
   * - or
     - :math:`l_{ix} < x_i < u_{ix}`
     - and
     - :math:`f_i(x) = 0`


A complementarity condition modeled in AIMMS is transformed into this formulation. Note that no transformation of the complementarity condition is needed if
:math:`l_{if} = -\infty` and :math:`u_{if} = \infty`.


PATH requires that the mixed complementarity problem is square (i.e., the number of variables and constraints must be equal) and PATH cannot handle normal inequalities (i.e., inequalities that have no complemented variable). On the other hand, AIMMS does not require that the mixed complementarity problem is square and AIMMS allows that normal inequalities are included. Therefore a mixed complementarity problem defined in AIMMS has to be transformed into the input format needed by PATH. AIMMS will match unassociated variables to 'normal' inequalities, and make the problem square by adding variables or constraints. However, users should avoid normal inequalities if possible and match unassociated variables and normal inequalities when the matching makes sense for their application! Structure and convexity can be destroyed if it is left to the AIMMS to perform the matching, which can have a negative influence on PATH's performance.



PATH is equipped with parameters that influence its performance. AIMMS is equipped with options that set the parameters in PATH. Options in AIMMS can be set in the options dialog box.



**Learn more about** 

*	:ref:`PATH_Path_to_AIMMS_Mapping`  
*	:ref:`PATH_AIMMS_to_Path_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	:ref:`sec:compl.variable`  



