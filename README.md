Analysis Output and methodology

## How did we define our cohort?
Our study population was intended to represent patients within the Connected Bradford database who have or might have complex mental health difficulties. As such, it comprises anyone with mental ill-health but who does not have a diagnosis of a serious mental illness (specifically, schizophrenia or bipolar disorder). This was  defined as:
- any person with a record in the primary-care tables within the Connected Bradford database;
- aged between 18 and 70, inclusive;
- who have been registered with their general practice for at least one year;
- who, additionally, either have a record of a SNOMED-CT diagnostic code of interest within ten years prior to 31st December 2021, and who have a record of prescriptions for medicines of interest within ten years prior to 31st December 2021;
- but excluding those people who have a record of a SNOMED-CT diagnostic code of schizophrenia or bipolar disorder.

Our codelist of SNOMED-CT diagnostic codes for [mental ill-health is available from opencodelist.org](https://www.opencodelists.org/codelist/user/ciaranmci/mental-disorder/5c00ffcc/). Our codelist for [schizophrenia is available here](https://www.opencodelists.org/codelist/user/ciaranmci/schizophrenia/37e4226d/) and our codelist fo [bipolar disorder is available here](https://www.opencodelists.org/codelist/user/ciaranmci/bipolar-disorder/6a0308d7/). Our medications of interest are shown below:
- Risperidone
- Olanzapine
- Quetiapine
- Flupentixol
- Diazepam
- Zopiclone
- Clomipramine
- Citalopram
- Duloxetine
- Escitalopram
- Mirtazapine
- Paroxetine
- Sertraline
- Trazodone
- Venlafaxine
- Fluoxetine
<br/>
<br/>
<br/>

## What has been uploaded?
To this repository, we have uploaded:
- a folder containing all codelists used by other scripts for defining features and our target variable.
- a Jupyter notebook that defines all our user-defined functions.
  - UNSEEN_helper_functions.ipynb
- all Jupyter notebooks necessary to identify the study population and to create the target variable representing the caseness of complex mental health difficulties.
  - UNSEEN_create_caseness_variable.ipynb
- all Jupyter notebooks necessary to create the variables representing the candidate features within electronic healthcare records that we evaluate for their association with our target variable.
  - UNSEEN_create_feature_sets_base.ipynb
  - UNSEEN_create_feature_sets_appendix1.ipynb
  - UNSEEN_create_feature_sets_appendix2.ipynb
  - UNSEEN_create_feature_sets_appendix3.ipynb
  - UNSEEN_create_feature_sets_appendix4.ipynb
  - UNSEEN_create_feature_sets.ipynb
- all Jupyter notebooks necessary to evaluate the candidate features that we created.
  - UNSEEN_evaluate_feature_sets.ipynb
- several scripts that record mini-studies and adjacent data processing that helped us to understand the data and our findings.
  - UNSEEN_cluster_study.ipynb
  - UNSEEN_simStudy_MIandMisclassification.ipynb
  - UNSEEN_visualise_feature_set_distributions.ipynb
  - UNSEEN_caseness_cohort_breakdown.ipynb
  - UNSEEN_prescription-based_caseness_over_time.ipynb
  - UNSEEN_prescribing_trends.ipynb
  - UNSEEN_patients_with_Rx_over_time.ipynb
  - a Jupyter notebook summarising our main findings.
  - UNSEEN_report_results.ipynb

All scripts are written in Jupyter notebooks, almost exlcusively in Python, but with some R.  
<br/>
<br/>
<br/>


## What has it been used for?
To date, this work has informed draft academic publications and a stakeholder meeting in which patient and professional representatives of mental health services discussed the findings and the development of both recommendations and a toolkit to help mental-health services provide for people experiencing complex mental health difficulties.
<br/>
<br/>
<br/>

## Who would use it?
Understanding Services for people with Complex Mental Health Difficulties (UnSeen) is a mixed-methods project involving a qualitative study of patients’ and general practitioners to examine how practitioners conceptualise complex mental health difficulties and how patients describe, understand and make sense of them ([NIHR203473](https://fundingawards.nihr.ac.uk/award/NIHR203473)). The project’s qualitative work informed the quantitative study described in this repository, which asks _What features within patients’ primary-care electronic health records might indicate that a patient has “complex” mental health difficulties?_ We will combine the features that we have identified with other insights from the project's qualitative work package to provide recommendations to mental health services and general practices on how to identify and help people experiencing complex mental health difficulties.
