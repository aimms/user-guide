

.. _Miscellaneous_State_File_Manager:


State File Manager
==================

**Description** 

When using Pivot Table(s) in your project, you can save the layout/state of the Pivot Table into a state file. With the State File Manager, that can be found in the Tools menu, the developer of a project can manage the states that are stored in any of the state files.



In the State File Manager dialog box, you can select one of the state files that come with your project: Main Project (Developer State), User State, and possibly one or more Library state files.



The table displays the states that are stored in the selected state file. It shows the name of the state, which can either be: 

*	A UUID (e.g. 7011984C-0B27-4DEE-97C4-F64F0793592E). In case no state name was specified, AIMMS generates such a UUID as state name when saving a state. 
*	A string specified via the :ref:`Pivot-Table_General2`  properties on the General tab of the Pivot Table properties dialog box. This can either be a string parameter or a quoted string.




Furthermore, the table displays the size of the state. In case your state file takes a lot of memory, you can use the State File Manager to see which states use a lot of memory.





You can also see on which page a certain state is used. The values in the Used on Page column can be:

*	**A page name:**  the name of a page in your project on which a Pivot Table is located in which the given state name is referred to literally (so not via a string parameter). In this case, the **Open Page** button becomes active when you select such a state. You can use it to open the page on which the state is used.
*	**Not Used!**  This status only appears for names that are UUIDs. You might want to delete these states, because they correspond to e.g. Pivot Tables on pages that no longer exist. You can select all unused states for the selected state file by pressing the **Select All Unused**  button, after which you can press the **Delete** button to delete the selected states.
*	**Unknown:**  If the name of the state is not a UUID and the name was not referred to literally in any of the Pivot Tables, it is not known on which page the state is used. Since state names can be specified via a string parameter, it could be that it is in use through such a string parameter.




**Learn more about** 

*	The :ref:`Pivot-Table_General2`  properties on the General tab of the Pivot Table properties dialog box.
*	The Search for Pivot Table State functions that can be found in the AIMMS Function Reference. These functions can also be used to save, load or delete states.



