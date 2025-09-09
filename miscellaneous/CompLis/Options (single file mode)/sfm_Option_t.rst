.. _sfm_Option_t:
.. _CompLis_sfm_Option_t:

Option 't'
==========

**Usage** :	CompLis <filename> -t [l<n>] [u<n>]	

If this option is set then CompLis will display the smallest and largest coefficient (in absolute sense).

The optional argument 'l' can be used in combination with option 't' to display all coefficients smaller than the value behind 'l'. In the same way the optional argument 'u' can be used to display all coefficients larger than the value behind 'u'. For example, '-t l1e-8 u1000' means that all coefficients smaller than 1e-8 and larger than 1000 (in absolute sense) will be printed. In that case the output might look like:

.. code-block:: none
    :linenos:

    File 'sc.lis' (small value = 1.00E-008; large value = 1.00E+003):

    Listing 1 (first of SCModel):
    --------------------------
    *** The largest coefficient (in absolute sense) = 1.11E+004
    *** The smallest coefficient (in absolute sense) = 5.62E-009    

    GenerationIncidenceDetermination(London,England):
       coefficient for variable Generation(Paris,France) is small (-7.22E-009) 
    GenerationIncidenceDetermination(Paris,France):
       coefficient for variable Generation(Rome,Italy) is large (-1.11E+004)

Line 1 shows that 1e-8 is used for argument 'l' and 1000 for argument 'u'. 
Line 3 shows that infomation is printed for the first constraint listing. 
Lines 5 and 6 show the largest and smallest coefficient in the constraint listing.

Line 8 shows the name of a constraint in which a small coefficient was found, namely the coefficient 
for variable 'Generation(Paris,France)' as shown in line 9. Line 10 shows the name of a constraint 
in which a large coefficient was found, namely the coefficient for variable 'Generation(Rome,Italy)' as shown in line 11.



