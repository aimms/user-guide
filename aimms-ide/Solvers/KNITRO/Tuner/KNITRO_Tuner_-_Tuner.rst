.. _option-KNITRO-tuner:


Tuner
=====



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	



This option determines whether to invoke the Knitro-Tuner. Possible values are:



    *	Off
    *	Automated
    *	Customized




A description of the Knitro-Tuner can be found in the :doc:`KNITRO_Tuner_-_Tuner`  section. Setting 'Automated' will cause Knitro to automatically run your model with a variety of automatically determined option settings. With setting 'Customized' you can tell Knitro which options you want it to tune (as well as specify the values for particular options that you want Knitro to explore); this is done through the Tuner options file.





**Learn more about** 

*	:doc:`KNITRO_Tuner_-_Tuner` 
*	:doc:`KNITRO_Tuner_-_Tuner_Output`  
*	:doc:`KNITRO_Tuner_-_Tuner_Terminate`  
*	:doc:`KNITRO_Tuner_-_Tuner_Time_Limit`  
