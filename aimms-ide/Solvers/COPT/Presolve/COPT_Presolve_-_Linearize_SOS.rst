.. _option-COPT-linearize_sos:


Linearize SOS
=============



:Type:	Selection	
:Range:	The settings listed below	
:Default:	Automatic	



This option controls whether to force the linearization of SOS constraints, in which case
SOS constraints will be transformed into equivalent linear constraints. Possible values are:

    *	Automatic
    *	Off
    *	On


If this option is set to 'Off' then COPT does not not force the linearization of SOS constraints.
If this option is set to 'On' then COPT forces the linearization of all SOS constraints.

At the default setting COPT attempts to linearize SOS constraints when the model is numerically
well-conditioned.
