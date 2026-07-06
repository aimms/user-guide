.. _option-ODHCPLEX-sos_in_key:


SOS in Key
==========



:Type:	Selection
:Range:	The settings listed below
:Default:	Treat SOS members as normal



This option specifies whether each Special Ordered Set (SOS) is assigned to its own sub-model component (key). Possible values are:



    *	Treat SOS members as normal
    *	SOS members always in keys
    *	Always in keys, each SOS in own key




With setting 'Treat SOS members as normal', SOS members are only placed in keys if they are declared non-continuous, or if all variables are included (see option **Integer Only**).

With setting 'SOS members always in keys', SOS members are always placed in keys.

With setting 'Always in keys, each SOS in own key', SOS members are always placed in keys and the members of each SOS are assigned to their own key.




**Note**

*	This option was added in ODH-CPLEX 8.2.




**Learn more about**

*	:doc:`Advanced - Integer Only <ODH_Advanced_-_Integer_Only>`
