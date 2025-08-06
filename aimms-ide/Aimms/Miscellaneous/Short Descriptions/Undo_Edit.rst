.. |img_def_Undo_button_bmp| image:: images/Undo_button.bmp


.. _Miscellaneous_Undo_Edit:


Undo Edit
=========

**Description** 

When you have made changes to any of the data on a page, and you want to undo the latest changes, AIMMS offers the end-user two undo commands:

*	If you select |img_def_Undo_button_bmp| Undo Last from the Edit menu, then the last data change is undone. At the same time, the data change just before the last becomes the last data change, so you can execute the command consecutively to undo a whole series of changes.
*	If you select Undo… from the Edit menu, AIMMS will show a dialog box in which a list of the last data changes is displayed. In this list you can select the data change up to which you want to undo.




**Note** 

*	AIMMS maintains a list of data changes that you can still undo at a certain point. This list is emptied when you invoke an action that changes many data at once (for example when loading a case or running a procedure that changes data). If your model contains procedures that do change data, but you do not want the undo list to be cleared, you can mark these procedures via the property UndoSafe.



