

.. _Bar-Chart_Object_Properties_Procedure:


Procedure
=========

**Description** 

In the Procedure tab of the object property dialog box, you can specify procedures to be run either when the user changes a value in an object or when he changes the selection/focus in the object. If the object contains multiple identifiers, you should specify the procedures for each individual identifier.



**Upon Data Change** **–** **Procedure** 

This procedure is executed whenever the user makes a change in the data that is displayed in the object. The procedure that you specify should either be a procedure without any arguments, or a procedure with element parameter arguments. These element parameter arguments should then match the indices of the identifier in the object. For example, if the object contains the identifier A(i), then you can use a procedure MyProcedure(elemparam), where the range of elemparam corresponds to the set of index i, and specify this procedure as follows: MyProcedure(i). If the user then changes the value of A('i01'), the procedure will be called via MyProcedure('i01').



In the table object, the user can make multiple data changes at once (by selecting a whole block of cells). Therefore, the Procedure tab lets you specify whether the procedure upon data change should be executed for every individual data change, or only once after all changes have been made.



**Upon Data change - Update** 

Besides running a procedure whenever the user makes a change in the data, you can define that a specific identifier with a definition is updated. This is only relevant if this identifier is not updated automatically (i.e. not an element in the pre-defined set CurrentAutoUpdatedDefinitions). By default, all defined identifiers are updated automatically when needed, so usually you do not need this option.



**Upon Selection** **–** **Procedure** 

This procedure is executed when the user changes the focus to the object or if he moves the cursor to another data entry within the object. Similar as for the Upon Data Change-Procedure, you can specify a procedure without any arguments or a procedure with element valued arguments.



To avoid numerous identical procedure calls when moving the cursor over the individual entries of an object, AIMMS stores the last executed procedure call and only executes the Upon Selection - Procedure if it differs from this last call. For example, if you have a table for a parameter A(i), and specify a procedure MySelectProcedure, then this procedure is only executed when the table first gets the focus, but not if you move the cursor around in the table (unless another procedure is executed in between). If you do want to run the procedure also when moving the cursor in the table, then you should extend the procedure with an element parameter argument and specify the procedure as follows: MySelectProcedure(i).



**Upon Double-Click** **–** **Procedure** 

This procedure is executed when the user double clicks in the object. Similar as for the Upon Data Change-Procedure, you can specify a procedure without any arguments or a procedure with element valued arguments. If you specify this procedure, a possible default right mouse popup menu item is ignored as double-click action.



**Learn more about** 

*	:ref:`Model-Explorer_Procedures` 
*	:ref:`Miscellaneous_Updatebility_of_Identifiers` 
*	:ref:`Page-Manager_Double_Click_in_Page_Object` 
*	:any:`CurrentAutoUpdatedDefinitions`






