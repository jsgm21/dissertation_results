# dissertation_results
Data dictionary 

These were the variables present in the data set used for traditional and time-dependent Cox regression analyses.
Some varaibles were calcualted or recalcualted from original UK-CRIS data sets. They will be identified with ** signs.

bcr_id - unique, anonimysed patient identifier

obsv_id** - unique identifier of each observation

Date_Of_Birth - patient's date of birth 

Gender_Value - patient's sex

Ethnicity_Value - patient's racial group

Marital_Status_Value - patient's marital status (6 groups)

marital_status** - patient's martial status regrouped (4 groups)

Date_Of_Death - patient's date of birth 

yyyy_mm** - year and month of the clinical records collated in one observation Used for merging of data sets

docdate_diag - date of clinical documents with mentions of dementia diagnoses 

type_diag - diagnoses recorded as dementia or MCI (MCI diagnoses were all excluded)

cause - specific dementia disease diagnosis (e.g., AD, Mixed, etc.)

negation_diag - whether prescription of medication was advised in clinical records of diagnoses 

severity - severity of dementia diagnoses. NLP model did not extract any information for this variable.

docdate_cog - date of clinical documents with mentions of dementia cognitive assessment scores 

type_cogeval - type of cognitive assessment administered 

numerator - score in cognitive assessment 

denominator - maximum points possible in cognitive assessment

negation_cogeval - whether prescription of medication was advised in clinical records of cognitive assessment scores

docdate_med - date of clinical documents with mentions of dementia medication

type_med - type of dementia medication prescribed 

negation_med - whether prescription of medication was advised in clinical records of dementia medication 

type_medother - type of chronic medication 

negation_medother - whether prescription of medication was advised in clinical records of chronic medication

docdate_medother - date of clinical documents with mentions of chronic medication

min_meddate** - date of first mention of dementia medication per patient

min_diagdate** - date of first mention of diagnosis per patient

brc_id2** - alternative patient identifier

obs** - index of observation per patient (e.g., a ptietn who had 4 observations would have their 1st observation indexed as 1, and their last observation indexed as 4)

type_medclass** - regroup of type_med used because of presence of unidentified AChEIs (2 groups)

type_medany** - revalue of type_med. Renamed all cases of any dementia medication into 'drug' mentions

any_demgrug - aggregate of type_medany per patient id 

first_demmed** - date of frist observation when medication was prescribed per patient. 

last_demmed** - date of last observation when medication was prescribed per patient.

type_diagper** - initial diagnosis recorded as dementia or MCI

cause_diagper** - initial specific dementia disease diagnosis 

first_diag** - date of first mention of diagnosis

med_status** - dementia medication use at currurent observation 

med_exposure** - recalculation of med_status. Whether patient was exposed to any dementia medication at current of observation

diag_status** - diagnosis recorded as dementia or MCI in current observation

cause_status** - dementia disease recorded in current observation

medother_grouped** - regroup of type_medother. Decreased number of groups of chronic medication. 

age_diag** - patient's age at time of frist diagnosis

min_dateobsv** - earliest date of clinical record present in an observation 

max_dateobsv** - latest date of clinical record present in an observation 

age_obsv** - patient's age at time of observation

date_entry** - patient's date of entry in cohort (i.e., date of first record ever assocaited to a pateitn identifier)

date_exit** - patient's date of exit of cohort (i.e., date of last record ever assocaited to a pateitn identifier)

age_entry** - patient's age at time of entry

age_entry** - patient's age at time of exit

time_surv** - patient's survival time in cohort

time_survob** - patient's remaining survival time at observation
