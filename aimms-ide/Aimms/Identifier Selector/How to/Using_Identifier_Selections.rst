

.. _Identifier-Selector_Using_Identifier_Selections:


Use Identifier Selections
=========================

**Description** 

You can use the identifier selections that are created from the selector nodes in several ways. The most obvious is to use the identifiers in a View Window, which can be done via the Open with command:

1.	Open the Identifier Selector.

2.	Select one (or more) nodes for which you want to view the identifiers.

3.	From the Edit menu, select Open with (or double click, see also remarks below).

4.	From the View Manager dialog box, select the View Definition that you want to use.

5.	(Check the Set as Default option, if you want to make this view the default for the selector node.).

6.	Click OK.



Besides the Open with command, you can use the selector nodes for various drag-and-drop operations to other AIMMS windows. In all these drag-and-drop operations it is best to remember that you are actually dragging a list of identifiers. This implies that you can drag to:

*	the Model Explorer, to find and highlight the positions of the identifiers in the model tree
*	a View Window, to either extend the list of identifiers that are displayed in the view or find and highlight the occurrences of the identifiers in the View Window. Here, the default drag-and-drop operation is to extend the list of identifiers in the View Window, if you want to find identifiers, you should hold down both the ``<Shift>``  and ``<Ctrl>``  keys during the drag-and-drop operation.
*	a Case Type or Data Category in the Data Management Setup tool, to add the identifiers to the contents of these nodes.
*	the Page Manager, Template Manager or Menu Builder, to find and highlight all nodes that contain references to any of the identifiers.
*	a page or template in Edit Mode, to find and select all objects that contain references to any of the identifiers.




**Remark** 


If you have defined a default view for a specific selector node, then double clicking on that node will directly open this default View Window (without showing the Open with dialog box). If you want to change this default view or just use another view for the selector node, then you should use the Open with command from the menu, which will always show the dialog box. If there is no default view selected, then double clicking is exactly the same as using the Open with command.

