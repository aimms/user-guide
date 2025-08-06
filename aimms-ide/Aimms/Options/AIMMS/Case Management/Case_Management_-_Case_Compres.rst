

.. _Options_Case_Management_-_Case_Compres:


Case Compression Level
======================



Type:	Integer	

Range:	{0..9}	

Default:	1	



This option determines what type of case compression should be used. Setting this option to "0" means that no case compression is used so that cases can still be read by older versions of AIMMS. The higher the setting of this option, the more the case will be compressed, but also the more time the compression will take. Please note that setting this option to 0 will make strings stored verbatim and thus make it more easy to extract information from the case without needing AIMMS.



