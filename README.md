# Validation of the model by Epic: Early Detection of Sepsis (EDS)

Please find the R-code used to perform the EDS evaluation in the file 
1. "EDSValidation_DataPreparation.R" to prepare the data for the analysis.
2. "EDSValidation_Epic.R" using the 8-hour time window, i.e., for patients without sepsis we use all the predictions of the full hospitalization and for patients with sepsis we use the 8 hours preceding sepsis onset.
3. "EDSValidation_TimeDependent" uses time-dependent measures. At each hour, we identify the highest prediction from the previous two hours and check whether sepsis occurred within the following eight hours.

You can find the Figures resulting from this R-code in the folder "Figures". The data can be requested from Josh Choi (Josh.Choi@tuftsmedicine.org).
