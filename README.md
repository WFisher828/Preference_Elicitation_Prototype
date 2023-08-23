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
3. g_opt_multi_lvl
4. two_stage_g_opt
5. two_step_g_acq (WE INCLUDE THIS HERE BECAUSE IT DEPENDS ON moment_matching_update AND g_opt, THEMATICALLY THIS
SHOULD NOT BE HERE)
6. multlvl_two_step_g_acq (WE INCLUDE THIS HERE BECAUSE IT DEPENDS ON moment_matching_update AND g_opt_multi_lvl, THEMATICALLY THIS
SHOULD NOT BE HERE)

The module "Experiment_Framework" has functions which are used in conducting numerical experiments. These functions include:
1. product_diff_list
2. multlvl_product_diff_list
3. question_extractor
4. multlvl_question_extractor
5. enum_two_step
6. multlvl_enum_two_step
7. enum_two_step_opt
8. quantile_test_enum_data
9. one_step_sol_two_step_quantile
10. multlvl_one_step_sol_two_step_quantile
11. MSE_det_test 
12. new_sequential_experiment (!!!THIS CODE NEEDS TO BE CHECKED IN DETAIL!!! PARTICULARLY DEALING WITH THE GUMBEL ERROR TERM)

The module "Batch_Design_and_Rollout" has functions which are used in creating a batch design of questions with certain orthogonality conditions,
as well as functions which are used in performing rollout on a question pair. Rollout is a non-myopic method often used in solving dynamic programming problems. 
These functions include:
1. orthogonal_constraint_feas
2. batch_design_delta_penalty #THIS WILL BE PREFERRED OVER batch_design_delta_refine
3. batch_design_AO
4. batch_design_MO
5. batch_design_delta_refine
6. question_selection_prob
7. rollout
8. monte_carlo_rollout
9. rollout_with_batch_design_acquisition
10. coordinate_exchange_acq
