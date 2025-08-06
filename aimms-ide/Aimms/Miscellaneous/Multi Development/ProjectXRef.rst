

.. _Miscellaneous_ProjectXRef:


Project Cross References
========================



**Description** 

In the Project Cross References dialog you can analyze the cross references between the main project and different library projects. This dialog can be accessed via the menu Tools - Cross Library References. This tool can be used to help you subdivide your application into different library projects and remove any unwanted references.



On the Usage of Local Declarations tab you find a list of items from the selected project that are referred in other projects, with the item name, the name of the other project it is used in, and the tool in the other project it is used in. The Show Where button can be used to open the selected tool in the other project at the position of the reference.



In the Usage of External Declarations tab you find a list of items from other projects that are referred to in the selected project, with the item name, the name of the other project and the tool it is used in. The Show Where button can be used to open the selected tool in the project at the position of the reference.



On the Settings tab you can specify which project you want to consider for the comparison and which type of references to consider. 



On the Settings tab you can also specify so-called Preferred References. These preferred references can help you to inspect and manage the references between several libraries. If you rather do not want references from library A to library B, then you can exclude this type of reference in the Preferred References. In the current AIMMS versions this does not change anything in how your AIMMS application works. The effect of changing the Preferred References is only visible in the Cross References dialog itself, in the way that any existing non-preferred reference is displayed in red or is marked with a series of stars ``****`` when printed out. Initially, all references between libraries are included in the Preferred References.



