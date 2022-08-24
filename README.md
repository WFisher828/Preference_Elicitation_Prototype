# Preference_Elicitation
A collection of code for the Preference_Elicitation Project

The module "Baseline_Functions_Definitions" includes functions that the questionnaire procedure and experimental framework
are based off of. The functions include:
1. z_expectation_variance
2. g_fun
4. g_fun_linear_regression

The module 'Questionnaire_Procedure' has all of the functions needed to do one-step and 
two-step questionnaire, along with the two-step acquisition function since it depends on functions
coming from this module. It includes the following functions:
1. moment_matching_update
2. g_opt
3. two_stage_g_opt
4. two_step_g_acq (WE INCLUDE THIS HERE BECAUSE IT DEPENDS ON moment_matching_update AND g_opt, THEMATICALLY THIS
SHOULD NOT BE HERE)
