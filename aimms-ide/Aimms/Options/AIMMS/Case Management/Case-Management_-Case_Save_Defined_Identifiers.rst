

.. _option-AIMMS-case_save_defined_identifiers:


Case Save Defined Identifiers
=============================



:Type:		Selection	
:Range:		The settings listed below	
:Default:	The default for this option is on



This option determines whether identifiers with a definition will be stored explicitly in a case. 



If you simply want to store a case to be able to load it back in later, it is not necessary to store the data of defined identifiers. Because, during a standard case load, the data of the defined identifiers is just skipped and the definition will be re-evaluated with the newly read data of the identifiers on which it depends. 



The only reason to save defined identifiers is when you use the saved case also in a 'multiple case' scenario. For example if you want to compare the data of multiple cases, you can only compare the data of defined identifiers if these identifiers are explicitly stored. This is because AIMMS is not able to evaluate a definition for a case that is not the active case.

So when you use case comparison features of the WebUI, or use the case-dot notation on identifiers with a definition you probably want to keep this option on the default value ('On').



If you don't need this, then setting it to 'Off' may have a positive effect on both the size of the case file and the time it takes to save the case. This is because prior to saving the defined identifier will be made up-to-date and thus takes execution time. See also the option :ref:`option-AIMMS-save_data_update_definitions` .



To have even more control over which (defined) identifiers should not be included in a case file you can also set the property 'NoSave' on each identifier.





Possible values are:



    *	Off (do not include identifiers with a definition)
    *	On (include identifiers with a definition)



