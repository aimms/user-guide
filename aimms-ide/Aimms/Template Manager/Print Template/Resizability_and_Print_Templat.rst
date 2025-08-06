

.. _Template-Manager_Resizability_and_Print_Templat:


Resizability and Print Templates
================================

**Description** 

You can create a resizable print page by adding resize split lines to the page. You can add split lines in a similar way as for normal end-user pages, but an important difference lays in the use of the User Adjustable split lines.

If you place a User Adjustable split line on a normal end-user page, the user can drag this line in order to see more or less of a specific area in the page and, if the user double-clicks on the line, the line will be positioned such that the objects at one side of the line are completely visible (unless the page itself is not large enough).

On a print page a User Adjustable line has a behavior similar to the user's double click, except that this double click is done by AIMMS itself. Just before printing or previewing a (next) output page, the print operation itself will move the user adjustable split lines to the most suitable position. For example, if you place a User Adjustable split line just below a table on your page, then before printing the page this line will be positioned such that as much as possible of the table data is printed on that output page. If there is still not enough space to display all data, then on the next output page, the resize line will again be positioned such that as much as possible of the remaining data of the table is printed, and so on.



**Learn more about** 

*	:ref:`Page-Manager_Resizability_Introduction` 



