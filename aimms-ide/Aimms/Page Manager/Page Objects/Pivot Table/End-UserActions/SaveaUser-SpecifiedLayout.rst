

.. _Pivot-Table_SaveaUser-SpecifiedLayout:


Save a User-Specified Layout
============================

The current layout of the pivot table is referred to as the User State. The developer of the pivot table may decide whether or not the end-user is allowed to store his layout in a so-called user-state file. In addition, the developer may control the amount of detail that is stored in the user-state file as well as the moment on which the user-file is stored.



If the developer has indicated that the end-user is responsible for saving his own user state, the end-user can store the user state through the Save User State menu command (in the View menu of a page in User Mode). The option to control this and the specification of what information should be saved in the state file can be found on the General tab of the pivot table options dialog. 



**Remark** 

 

When using pivot table pages in combination with libraries, please note the following. When dragging a page (with pivot table) from the main model to a library, AIMMS will not automatically store the layout of the pivot table in the developer state file of the library. This will only happen once the page is resaved. Because of this it is advised to resave all pages in a library after moving them to the library, to prevent loss of layout.



**Learn more about** 




*   :ref:`Pivot-Table_General2` 


*   :ref:`Pivot-Table_Load_a_Layout` 





