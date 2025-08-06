

.. _Indexed-Page_Indexed_Page_Object_Propertie1:


Indexed Pages
=============

**Description** 

In the indexed pages tab, you can adjust the following properties:



**Page to Show** 

You can specify the page that is shown in the indexed page object. You can enter the name of the page, or select a page by using the wizard.



**Page Layout** 

You can select one of the following four page layouts:

1.	Row Wise, the shown pages fill the indexed page object row by row.

2.	Column Wise, the shown pages fill the indexed page object column by column.

3.	Matrix, the shown page depends on two different element parameters.

4.	Single Page, the page to show is shown once, for the current value of the element parameter.



**Inter Page Spacing** 

The inter page spacing is the amount of space between two pages in the indexed page object. This property cannot be specified when Single Page is selected as Page Layout.



**Always Hide Scrollbars** 

For some usages of the indexed page object, you know that a scroll bars will never be needed. By setting this option the object does not need to decide on the display of a scroll bar, and prevents it from sometimes displaying a scroll bar very shortly.



**Index Rows by Parameter:** 

When Row Wise, Column Wise or Matrix is selected as Page Layout, an element parameter must be specified. The Page to Show will be displayed for all values in the range of that element parameter. This should be dependent of the element parameter. It is recommended to use a dedicated element parameter for this setting, and to only use this parameter on the page as a slice of an indexed identifier, as part of a GUI expression, or displaying the element parameter itself.. If you use it in for example definitions of identifiers that you show on the indexed page, you will get inconsistent behavior.



**Index Columns by Parameter:** 

When Matrix is selected as Page Layout, two element parameters must be specified. The Page to Show will be displayed for all values in the range of both element parameters. This page should be dependent of both element parameters. The second element parameter can be entered at Index Columns by Parameter.



**Use as Reverse Link** 

When this property is selected, the end user is able to select the value of the element parameter by clicking on one of the pages in the indexed page object. This can be used to show more information about the current value of the element parameter.



**Rows:** 

At Rows you can choose whether you want a fixed number of rows in the indexed page object, or that the number of rows depends on the page height of the shown page.



**Columns** 

At Columns you can choose whether you want a fixed number of columns in the indexed page object, or that the number of columns depends on the page width of the shown page.





