

.. _option-AIMMS-warning_time_consuming_for_threshold:


Warning Time Consuming For Threshold
====================================



:Type:	Integer	
:Range:	{0 .. :ref:`Miscellaneous_Maxint`}	
:Default:	64	



In the case that the indices of a for loop have a specified element order, the condition of the for loop is changed
by the statements inside the for loop, and the cardinality of the indices is large, the evaluation of the condition
and the statements inside the for loop may become time consuming. This can happen because each time the condition of
the for loop is changed, it has to be re-evaluated. When the cardinality of the indices (this is the number of indices
for which the condition has to be checked each time) is large, this can be a time consuming process. In such a case a
warning that this for loop may be the cause of the waiting is issued when the cardinality is larger than the value of
this option. 

In order to make your application more efficient there are several ways to improve this for loop. It is then necessary,
however, to understand a little bit about the execution strategies available to AIMMS to evaluate such a loop, as each
strategy has its own merits and drawbacks.

Consider the for loop:

.. code-block:: text

    for ( (i,j,k) | Expr(i,j,k) ) do
        statements ;
    endfor ;


whereby i,j,k are indices into the sets S, T, U each with a specified ordering and Expr is some expression over the indices i,j,k.

The first strategy, called the sparse strategy, will evaluate Expr completely before doing any of the statements and then for each
tuple (i,j,k) != 0.0 execute the statements. If an identifier is modified during the execution of these statements, then the condition
Expr will need to be re-evaluated completely.

The second strategy, called the dense strategy, evaluates Expr for each possible combination of index values of (i,j,k). As soon
as a non-zero result is found the statements are executed. Re-evaluation is avoided at the price of considering every combination of (i,j,k).

The third strategy, called the unordered strategy, uses the normal sparse execution engine of AIMMS ignoring the order of the indices.
This may, however, give different results, especially when the for loop contains a display/put statement or uses lag and lead operators
in conjunction with one or more of the ordered indices.

AIMMS uses the sparse strategy by default and only issues a warning if an identifier referenced inside the for loop is actually modified
and the second evaluation of Expr gives a non-empty result.

Considering the above you have the following options to improve the for loop:

    * rewrite Expr and statements, such that the condition does not change during the for loop.
    * prefix the for loop with the keyword UNORDERED. In that case the unordered strategy is chosen. You can do this if the element ordering is not relevant to the for loop.
    * prefix the for loop with the keyword ORDERED. In that case the dense strategy is chosen. You can do this if Expr contains a significant portion of all possible combinations of (i,j,k).
    * prefix the for loop with the keyword SPARSE. In that case the sparse strategy is chosen, but this warning is suppressed. You can do this if only in a few iterations an identifier in the condition is modified.

