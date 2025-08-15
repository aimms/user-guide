

.. _Options_Case_Management_-_Case_Compati_2:


Case Compatibility
==================



**Type**:	Selection	

**Default**:	Aimms 3 14	



This option determines whether the cases should be compatible with older versions of AIMMS. 

To be able to make constant improvements to AIMMS, it is sometimes necessary to change the way cases are stored. It is always possible to read cases made with an older AIMMS version, but it is by default not always possible to read cases made with a newer AIMMS version. If you want to be able to read cases in an older AIMMS version, you should modify this option. 



Possible values are:

*	Aimms_3_14
*	Aimms_4_80 (improved ordering of identifiers in a case, for better performance, and this is required if you want to use the Native_Linux or Native_Windows character encodings. See :ref:`Options_Case_Management_-Case_String_Character` 




**Remark** 


We advice you to set this option to older versions only if the cases need to be compatible with older versions of AIMMS.





**Learn more about** 

*	:ref:`Options_Case_Management_-_Case_Compres`  



