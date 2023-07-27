# Random-create-simple-EHR-data
This is a python script which used to produce fake EHR data in New York City.
The Python script generates multiple DataFrames to simulate medical information. Here are the details of the data ranges and randomization for each DataFrame:

person_df: Contains 1500 rows representing individuals' personal information.

Year_of_birth: Dates of birth range from 75 years ago to 10 years ago, randomly generated using generate_data function.
Race: Randomly selected from ["Asian", "African", "Caucasian", "Hispanic", "Other"] for each person.
Gender: Randomly selected from ["Male", "Female"] for each person.
FIPScode: Randomly selected from [36005, 36047, 36061, 36081, 36085] for each person.
visit_occurrence_df: Contains 7000 rows representing visit occurrences.

Visit_start_date: Dates range from 8 years ago to 7 months ago, randomly generated using generate_data function.
Visit_end_date: For outpatient visits, the end date is set to be the same as the start date.
Visit_type: Randomly selected from ["ED", "inpatient", "outpatient"] for each visit.
condition_occurrence_df: Contains 7000 rows representing medical condition occurrences.

Condition_start_date: Dates range from 8 years ago to 7 months ago, randomly generated using generate_data function.
Condition_end_date: For each condition, a random duration of 1 to 14 days is added to the start date to generate the end date, limited to a maximum 2-week condition period.
Condition_name: Randomly selected from the list of condition names for each condition occurrence.
drug_exposure_df: Contains 7000 rows representing drug exposure events.

Drug_exposure_start_date: Dates range from 8 years ago to 7 months ago, randomly generated using generate_data function.
Drug_exposure_end_date: For each drug exposure, a random duration of 1 to 14 days is added to the start date to generate the end date, limited to a maximum 2-week exposure period.
Drug_name: Randomly selected from the list of drug names for each drug exposure.
procedure_occurrence_df: Contains 7000 rows representing medical procedure occurrences.

Procedure_date: Dates range from 8 years ago to 7 months ago, randomly generated using generate_data function.
Procedure_name: Randomly selected from the list of procedure names for each procedure occurrence.
respiratory_related_procedure: A flag indicating whether the procedure is related to the respiratory system, based on predefined respiratory-related procedures.
The data is randomly generated within the specified date and name ranges to simulate diverse medical records for analysis and healthcare applications.
