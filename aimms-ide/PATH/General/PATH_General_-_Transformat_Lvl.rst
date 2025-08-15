.. _PATH_General_-_Transformat_Lvl:


Transformation Level
====================



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Advanced transformation	



This option determines how complementarity problems defined in AIMMS are transformed into the input format that PATH needs. In case of a 'Standard transformation' this transformation is trivial. If the value of this option equals 'Advanced transformation' (the default setting) the model passed to PATH is more adapted to 'normal' inequalities; PATH seems to handle the formulation following from this transformation (instead of the 'Standard transformation') better. If the value equals 'More advanced transformation' the model passed to PATH is more adapted to so-called unassociated variables (i.e. variables in AIMMS that are not a complementarity variable). Possible values are:



*	Standard transformation
*	Advanced transformation
*	More advanced transformation






