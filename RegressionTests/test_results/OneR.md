Single Rule Classification (`OneR`)
 ===== 

There are regression tests to compare model results between different versions of `caret` and the individual packages. These test evaluate whether consistent results can be obtained. The code used to generate the objects that are compared can be found [here](https://github.com/topepo/caret/blob/master/RegressionTests/Code/OneR.R).

Testing Information:
---------

Old:

 * x86_64-apple-darwin13.4.0 (64-bit)
 * R Under development (unstable) (2015-11-18 r69655)
 * `caret` (6.0-62), `RWeka` (0.4-24)
 * tested on 2015-12-31 at 17:28


New:

 * x86_64-apple-darwin13.4.0 (64-bit)
 * R Under development (unstable) (2015-11-18 r69655)
 * `caret` (6.0-64), `RWeka` (0.4-24)
 * tested on 2016-01-04 at 14:11


Results:
---------

**Test Case**: `class_cv_form`

Object class(es): `train` and `train.formula`

Model Configuration:

 * Formula method
 * Resampling: Cross-Validated (3 fold)
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 1 tuning parameter combination was evaluated


Execution times: (old) 0.96s (new) 0.99s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_cv_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: Cross-Validated (3 fold)
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 1 tuning parameter combination was evaluated


Execution times: (old) 2.03s (new) 2.12s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_loo_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: Leave-One-Out Cross-Validation
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 1 tuning parameter combination was evaluated


Execution times: (old) 5.13s (new) 5.27s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_none_model`

Object class(es): `train`

Model Configuration:

 * Non-formula method
 * Resampling: None
 * Grid search
 * Pre-processing: centered (7), scaled (7)  
 * 0 tuning parameter combinations were evaluated


Execution times: (old) 0.49s (new) 0.51s

Test Results:

 * _Equal results for ROC_
 * _Equal results for Sens_
 * _Equal results for Spec_

**Test Case**: `class_none_pred`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_none_prob`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `class_pred`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_pred_form`

Object class(es): `factor`

 * _Equal results_

**Test Case**: `class_predictors1`

Object class(es): `character`

 * _Equal results_

**Test Case**: `class_prob`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `class_prob_form`

Object class(es): `data.frame`

 * _Equal results_

**Test Case**: `levels`

Object class(es): `character`

 * _Equal results_

