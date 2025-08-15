.. _PATH_General_-_Merit_Function:


Merit Function
==============



**Type**:	Selection	

**Range**:	The settings listed below	

**Default**:	Fischer	



PATH employs a merit function to indicate the closeness of the current iteration point to the set of (feasible) solutions. The merit function is zero at a solution of the original mixed complementarity problem and strictly positive otherwise. In PATH the 'Normal Map function' or the 'Fischer function' (default setting) can be used as merit function. If the value of this option is 'Automatic', PATH itself chooses which merit function it should use. Possible values are:



*	Automatic
*	Normal
*	Fischer






