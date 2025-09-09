

.. _nm_Option_o:
.. _CompLis_nm_Option_o:


Option 'o'
==========

**Usage** :	CompLis <filename1> <filename2> -o	



If this option is set then CompLis will report ordering differences for constraints and variables.
In that case the output might look like:


.. code-block:: text
   :linenos:

    Comparing 'fac_loc_pn1.lis' vs 'fac_loc_pn2.lis' (options 'o'):
    
    MaxThroughputConstraint(Amersfoort):
       ordering differs (12 vs 11)	
    MaxThroughputConstraint(Gouda):
       ordering differs (11 vs 12)
       ordering of variable Served(Gouda,Maastricht) differs (2 vs 1)
       ordering of variable Served(Gouda,Haarlem) differs (3 vs 2)
       ordering of variable Selected(Gouda) differs (1 vs 3)


Line 4 shows that the constraint 'MaxThroughputConstraint(Amersfoort)' is the 12th constraint
in the first listing file and the 11th constraint in the second listing file. Line 6 shows that
for constraint 'MaxThroughputConstraint(Gouda)' it is the other way round, i.e., the two constraints
are swapped in the second listing file.


Lines 7, 8 and 9 show that the ordering of the variables in the constraint 'MaxThroughputConstraint(Gouda)'
is different. For instance, variable 'Selected(Gouda)' is the first variable in the constraint in the first
listing file but the third variable in the second listing file.

