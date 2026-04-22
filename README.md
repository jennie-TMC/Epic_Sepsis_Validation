# Validation of the model by Epic: Early Detection of Sepsis (EDS)
Code in this repo is adapted from and in collaboration with: https://github.com/CHMMaas/EDSValidation by Carolien Maas 

Please find the R-code used to perform the EDS evaluation in the file 
1. "EDSValidation_DataPreparation.R" to prepare the data for the analysis.
2. "EDSValidation_Epic.R" using the 8-hour time window, i.e., for patients without sepsis we use all the predictions of the full hospitalization and for patients with sepsis we use the 8 hours preceding sepsis onset.
3. "Time Dependent Analysis" folder uses time-dependent measures. At each hour, we identify the highest prediction from the previous two hours and check whether sepsis occurred within the following eight hours. The 2 files in this folder calculate time dependent measures with and without refractory periods.

You can find the Figures and measures resulting from this R-code in the folder "Results". The data can be requested from Josh Choi (Josh.Choi@tuftsmedicine.org).
