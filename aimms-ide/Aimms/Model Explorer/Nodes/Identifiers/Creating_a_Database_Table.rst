.. |img_def_Identifier_Database_Table_bmp| image:: images/Identifier_Database_Table.bmp
.. |img_def_Wizard_button_bmp| image:: images/Wizard_button.bmp


.. _Model-Explorer_Creating_a_Database_Table:


Creating a Database Table
=========================

**Description** 

To create a new database table in the Model Tree:

1.	Select the position in a Declaration Section where the new database table should be inserted

2.	From the Edit menu select Insert – Other (or press the ``<Insert>``  key)

3.	In the dialog box select |img_def_Identifier_Database_Table_bmp| Database table and press OK

4.	Enter a name for the new database table

5.	Press ``<Enter>``  to create the new database table (or press ``<Esc>``  to abort the operation)



The newly created database table is not yet ready for use, because you should at least specify some mandatory attributes. To modify the attributes of the newly created database table:

*	Press ``<Enter>``  or double click on the database table node.




The most commonly used attributes of a database table identifier are discussed below. 




*	``INDEX DOMAIN``  : The ``INDEX DOMAIN``  attribute should be specified in order to declare indexed database tables. The |img_def_Wizard_button_bmp| wizard will display the Set Dependency Tree of your model and allows you to select one or more indices.
*	``DATA SOURCE`` : The ``DATA SOURCE`` attribute should be used to specify the data source that will be used when communicating with the data provider (e.g. database). The data source contains information about how to connect to the data provider. This field can either contain a reference to an ODBC data source ( a dsn file or user/system data source), or a string parameter specifying one of these data sources. The |img_def_Wizard_button_bmp| wizard will display a menu allowing you to select either a File Data Source (dsn), a User/System Data Source or a string parameter from your model that will be used to specify the data source. When you select user/system data source a dialog will be opened in which you can select an ODBC Data Source. In this dialog you can also select a new data source or export an existing ODBC data source to a file data source. You can also configure your ODBC setup from the ODBC icon in the Windows Control Panel.
*	``TABLE NAME`` : The ``TABLE NAME`` attribute should be used to specify the name of the data table name that is communicated with. Typically a data source contains multiple data tables. The |img_def_Wizard_button_bmp| wizard will display a menu allowing you to select either an available data table or a string parameter from your model that will be used to specify the data table.
*	``MAPPING`` : The ``MAPPING`` attribute should be used to specify the relations between the data base columns and the AIMMS model identifiers. The |img_def_Wizard_button_bmp| wizard will display a dialog box allowing you to select columns in the specified data table and AIMMS identifiers.




**Learn more about** 

*	`Database tables and database table attributes <https://documentation.aimms.com/language-reference/data-communication-components/communicating-with-databases/the-databasetable-declaration.html>`_ (Language Reference)
*	:ref:`aimmshelp6-Model_Explorer_Attribute_Forms`  
*	:ref:`Model-Explorer_Attribute_Form_Manipulation`  



