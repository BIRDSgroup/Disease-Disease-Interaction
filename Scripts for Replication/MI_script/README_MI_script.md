# Instructions to run "MI_script.R" file
## Preface
This R file contains the code to reproduce the results from the Main and Interaction analysis.
The details of the outputs generated from this script are given below.

## Instruction
1. Modify the code at line 300 (shown below) to the working directory containing the main and interaction effect data.
```R
wd_m <- c("D:/work/DM_Hel/reproduce/data/")
```
2. After making this adjustment, save the script and execute it.

# Output from "MI_script.R"
Running this script will generate two folders **before_treatment** and **after_treatment** folders in the working directory that you have specified in the above section.
Here is the list of output files generated in both the folders:
|Output|Description|
|---|---|
|Ternary_plot|PNG image of Ternary plot|
|Main_effect_pvals|CSV file containing the list of features, p-values, and adjusted p-values from Main effect analysis|
|Interaction_effect_pvals|CSV file containing the list of features, p-values, and adjusted p-values from Interaction effect analysis|
|DATA_main_effect|Text file containing output from main effect analysis|
|DATA_interaction_effect|Text file containing output from interaction effect analysis|
|DATA_coeff|Text file containing the linear model (features regressed over covariates(including Diabetes and Helminth term)) outputs: model intercept, the coefficient for Diabetes term, and the coefficient for Helminth term|
|Coeff_terms_data|CSV containing features and their intercept, coefficient for Diabetes term, and coefficient for Helminth term from the linear model |
|per_exp_variance_BT(AT)|RDS file containing the list of features and the percentage of variance explained by the helminth term (class), diabetes term (group), and the interaction term. "per_exp_variance_BT" is for before-treatment samples and "per_exp_variance_AT" is for after-treatment samples.|
|rela_per_exp_variance_BT(AT)|RDS file containing the features and the relative percentage of variance explained by the helminth term (class), diabetes term (group), and the interaction term. "rela_per_exp_variance_BT" is for before-treatment samples and "rela_per_exp_variance_AT" is for after-treatment samples.|
|BT(AT)_mi_obj|list containing the main and interaction effect analysis output. "BT_mi_obj" is for before-treatment samples and "AT_mi_obj" is for after-treatment samples.|



