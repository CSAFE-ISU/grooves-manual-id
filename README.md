# grooves-manual-id
Storage and procedure for manual groove identifications on land engraved area (LEA) crosscuts. 

The file `manual_key.csv` contains a key for each manual groove identifier's "code" and their full name, in case anyone in the future needs to decipher the initials. For example, `manual_code = "kr"` and `manual_name = "Kiegan Rice"`. This will make the data a little more clean and consistent.  

There should be one single file for each bullet "study". Each file should be named `grooves_manual_studyname.rda` for clarity. For example, for Hamby Set 44, the file containing manual identifications is `grooves_manual_hamby44.rda`. Additional repetitions of manual identifications for a study already contained in the repository should be added to the existing `.rda` file, with the appropriate `manual_code` and `manual_rep` designations. 

Each `grooves_manual` file needs to contain the following columns: 

1. `study`: a short name for the study or set of bullets, which will also be included in the filename.  
    - e.g. `hamby44` for Hamby Set 44.
2. `source`: path to each data file on Sunny and/or Raven.  
3. `scan_id`: a unique identifier for each scan. This will be `barrel-bullet-land`, typically. 
    - e.g. `Barrel 1-Bullet 1-Land 1`, `Unknowns-Bullet 'K'-Land 1`
    - Note: for the Variability study, these need to include operator, machine, and round.
4. `crosscut`: Numeric value of the crosscut used for manual groove ID. This should result from `x3p_crosscut_optimize`. 
5. `manual_code`: Code identifying who completed the manual identification 
6. `manual_rep`: Repetition number within each individual's set of identifications.  
    - e.g. Kiegan did 3 repetitions on Hamby Set 44, so there are reps 1, 2, and 3.
7. `grooves_manual`: this is the vector obtained WITHOUT THE PLOT! For each scan, this should simply be a vector of 2 values (left and right manually identified groove).  

