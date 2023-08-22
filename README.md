# Preference_Elicitation (JUST SEEING HOW MERGE WORKS)
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

The module "Experiment_Framework" has functions which are used in conducting numerical experiments. These functions include:
1. product_diff_list
2. question_extractor
3. enum_two_step
4. enum_two_step_opt
5. quantile_test_enum_data
6. MSE_det_test 
7. new_sequential_experiment

The module "Batch_Design_and_Rollout" has functions which are used in creating a batch design of questions with certain orthogonality conditions,
as well as functions which are used in performing rollout on a question pair. Rollout is a non-myopic method often used in solving dynamic programming problems. 
These functions include:
1. orthogonal_constraint_feas
2. batch_design_delta_penalty #THIS WILL BE PREFERRED OVER batch_design_delta_refine
3. batch_design_delta_refine
4. question_selection_prob
5. rollout
6. monte_carlo_rollout
7. rollout_with_batch_design_acquisition
