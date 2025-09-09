

.. _sfm_Option_v:
.. _CompLis_sfm_Option_v:

Option 'v'
==========

**Usage** : CompLis <filename> -v [l<n>] [u<n>] 


If this option is set then CompLis will display the smallest and largest variable values (in absolute sense).
The AIMMS option **Constraint Listing Variable Values** should equal 'Print variable values' to create a
constraint listing containing the level values of the variables otherwise setting this option is useless.

The optional argument 'l' can be used in combination with option 'v' to display all variable values smaller
than the value behind 'l'. In the same way the optional argument 'u' can be used to display all variable values
larger than the value behind 'u'. For example, '-v l1e-7 u10000' means that all variable values smaller than 1e-7
and larger than 10000 (in absolute sense) will be printed. In that case the output might look like:

.. code-block:: none
    :linenos:

    File 'sc.lis' (small value = 1.00E-007; large value = 1.00E+004):

    Listing 1 (first of SCModel):
    --------------------------
    *** The largest variable level value (in absolute sense) = 2.31E+005
    *** The smallest variable level value (in absolute sense) = 2.62E-008   

    Generation(Paris,France):
       level value for variable Generation(Paris,France) is large (6.50E+004)  
    Generation(Rome,Italy):
       level value for variable Generation(Rome,Italy) is small (-3.33E-008)

Line 1 shows that 1e-7 is used for argument 'l' and 10000 for argument 'u'. Line 3 shows that infomation 
s printed for the first constraint listing. Lines 5 and 6 show the largest and smallest variable level
value in the constraint listing.

Line 8 shows the name of a variable that has a large variable level value, namely the level value as shown
in line 9. Line 10 shows the name of a variable that has a small variable level value, namely the level
value as shown in line 11.


**Learn more about** 

*	:ref:`option-AIMMS-constraint_listing_variable_values`

