

.. _option-AIMMS-generate_all_stage_0_stochastic_rows:


Generate All Stage 0 Stochastic Rows
====================================


:Type:	Selection	
:Range:	The settings listed below	
:Default:	Off	


This option determines, for a stochastic model, whether AIMMS should generate all stage 0 stochastic rows. Possible values are:


    *	Off
    *	On


If this option is set to 'On' then AIMMS will generate all stochastic rows if a constraint contains a stochastic parameter but no
stochastic variable, or if all stochastic variables are multiplied by 0 (zero). By default, AIMMS will only create one row, namely for
the representative scenario.


**Note** 

*	If a constraint contains a stochastic parameter but no stochastic variable then AIMMS will, by default, throw a warning, as controlled by the option **Warning Stochastic Programming Parameter without Variable**. This is also the case if this option is switched on.
*	If this option is switched off then AIMMS will, by default, do a consistency check on the scenarios in the stochastic program, as controlled by the option **Warning Stochastic Programming Scenario Consistency**.


**Learn more about** 

*	:ref:`option-AIMMS-Warning_stochastic_programming_parameter_without_variable` 
*	:ref:`option-AIMMS-warning_stochastic_programming_scenario_consistency` 
