

.. _Page-Manager_Expressions_in_the_GUI:


Expressions in the GUI
======================

**Description** 

Instead of using identifiers in a page object, it is also possible to use expressions. The use of expression in the graphical user interface can help you to keep the number of identifiers in your model to a minimum. 



You might consider using expressions instead of defined parameters whenever the information is only needed for the graphical user interface and not for the model itself. For example when you want to show a summation to the end-user, or when you want the visibility of an object to depend on a complicated expression.



When using expressions you should be aware of the following. An expression only contains data when the corresponding page is open. Compared to an identifier with a definition this means that an expression takes less memory. However an expression is evaluated again each time a page is opened, which might slow down the performance. 



The index domain of an expression does not depend on the context in which it is used. The best example of a situation one should pay extra attention to is when using an expression in a composite table. The index domain of the expression is not automatically limited to the domain of the composite table. When you place your expression between brackets and end it with $ followed by the index domain identifier/expression, you make sure that the expression is only evaluated for those tuples in the domain of the composite table. This prevents unnecessary memory usage or even execution errors.



**Learn more about** 

*	:ref:`Miscellaneous_Identifier_Selection_Dialog_Bo`  



