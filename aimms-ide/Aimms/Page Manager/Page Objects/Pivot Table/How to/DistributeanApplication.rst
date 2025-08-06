

.. _Pivot-Table_DistributeanApplication:


Distribute an Application with Pre-Defined Layout
=================================================

When distributing an application to an end-user a developer-state-file (if available) should also be shipped, the user-state-file not! When an update of the application (in which for example some identifier has been added to a pivot table) is shipped, again only the developer-state-file should be shipped. AIMMS will try to retrieve as much information from the user-state-file as possible and will use the developer-state-file as the fall-back state-file. Of course you should have made your application such that the user state is (or can be) saved (see the **General**  tab of the properties dialog box).



To make sure that the user layout is saved automatically, just set the **Save Layout/State - By End User**  option on the **General**  tab to "When page is closing" and set the **Save Layout/State - By Developer**  option to "No".



Whenever the application is run in developer mode and information for a pivot table is present in both a user and a developer-state-file, the developer-state-file is being used. When the application is run in end-user mode the user-state-file prevails. Pivot table information will only be read from one file (either the user-state-file or the developer-state-file). So, if the end-user added some aggregator and saved this information in a user-state-file and he receives an updated version of the application with a new version of some other pivot table (with some new identifiers and aggregators) the developer-state-file will not be used for this pivot table (and the new aggregator will not be visible). To force the developer-state-file to be used (and to ignore the user-state-file) the developer could decide to copy and paste the pivot table. The copied pivot table will be initialized with empty state files and therefore, changes made by the developer (that are stored in the developer-state-file) will not be overridden by some user settings (because no user state exists).



**Learn more about** 




*   :ref:`Pivot-Table_SaveaUser-SpecifiedLayout` 

