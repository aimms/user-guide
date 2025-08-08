
PATH
====

**Description** 

PATH is a tool for solving (square) mixed complementarity problems. Mixed complementarity problems are systems of linear and nonlinear constraints where variables in the model are linked to constraints in the form of mixed complementarity conditions. In AIMMS, a mixed complementarity condition is defined as follows for a given variable xi and an associated function fi(x).



If lif = -¥ and uif = ¥ then




.. list-table::

   * - 
     - either
     - xi = lix 
     - and
     - fi(x) ≥ 0
   * - 
     - or
     - xi = uix 
     - and
     - fi(x) ≤ 0
   * - 
     - or
     - lix < xi  < uix 
     - and
     - fi(x) = 0.


If lix = -¥ and uix = ¥ then




.. list-table::

   * - 
     - either
     - xi = 0 
     - and
     - lif < fi(x)  < uif 
   * - 
     - or
     - xi ≥ 0 
     - and
     - fi(x) = lif
   * - 
     - or
     - xi ≤ 0  
     - and
     - fi(x) = uif.


In any other situation, where exactly two of the constants lix, uix, lif and uif are finite, then




.. list-table::

   * - 
     - either
     - xi = lix 
     - and
     - lif ≤ fi(x)  ≤ uif 
   * - 
     - or
     - xi = uix 
     - and
     - lif ≤ fi(x)  ≤ uif 
   * - 
     - or
     - lix < xi  < uix 
     - and
     - fi(x) = lif
   * - 
     - or
     - lix < xi  < uix 
     - and
     - fi(x) = uif.




**Transformation** 

PATH uses a different definition. In PATH, a mixed complementarity condition requires that:




.. list-table::

   * - 
     - either
     - xi = lix 
     - and
     - fi(x) ≥ 0
   * - 
     - or
     - xi = uix 
     - and
     - fi(x) ≤ 0
   * - 
     - or
     - lix < xi  < uix 
     - and
     - fi(x) = 0.


A complementarity condition modeled in AIMMS is transformed into this formulation. Note that no transformation of the complementarity condition is needed if lif = -¥ and uif = ¥.



PATH requires that the mixed complementarity problem is square (i.e., the number of variables and constraints must be equal) and PATH cannot handle normal inequalities (i.e., inequalities that have no complemented variable). On the other hand, AIMMS does not require that the mixed complementarity problem is square and AIMMS allows that normal inequalities are included. Therefore a mixed complementarity problem defined in AIMMS has to be transformed into the input format needed by PATH. AIMMS will match unassociated variables to 'normal' inequalities, and make the problem square by adding variables or constraints. However, users should avoid normal inequalities if possible and match unassociated variables and normal inequalities when the matching makes sense for their application! Structure and convexity can be destroyed if it is left to the AIMMS to perform the matching, which can have a negative influence on PATH's performance.



PATH is equipped with parameters that influence its performance. AIMMS is equipped with options that set the parameters in PATH. Options in AIMMS can be set in the options dialog box.



**Learn more about** 

*	:ref:`PATH_Path_to_AIMMS_Mapping`  
*	:ref:`PATH_AIMMS_to_Path_Mapping`  
*	:ref:`Options_AIMMS_Execution_Options`  
*	Search for Complementarity Variable (Language Reference)



