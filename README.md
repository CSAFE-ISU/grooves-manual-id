# grooves-manual-id
Storage and procedure for manual groove identifications on land engraved area (LEA) crosscuts. 

The file `manual_key.csv` contains a key for each manual groove identifier's "code" and their full name, in case anyone in the future needs to decipher the initials. For example, `manual_code = "kr"` and `manual_name = "Kiegan Rice"`. This will make the data a little more clean and consistent. If your name/code are not already present, please add them to the file prior to uploading any manual groove data.  

There should be one single file for each bullet "study". Each file should be named `grooves_manual_studyname.csv` for clarity. For example, for Hamby Set 44, the file containing manual identifications is `grooves_manual_hamby44.csv`. Additional repetitions of manual identifications for a study already contained in the repository should be added to the existing `.csv` file, with the appropriate `manual_code` and `manual_rep` designations. 

Each `grooves_manual` file needs to contain the following columns: 

1. `study`: a short name for the study or set of bullets, which will also be included in the filename.  
    - e.g. `hamby44` for Hamby Set 44.
2. `source`: path to the relevant x3p file on Sunny and/or Raven.  
    - e.g. `/media/Sunny/CSAFE/Phoenix Set//Unknown 1-Y/L1.x3p`
3. `scan_id`: a unique identifier for each scan. This will be `study-barrel-bullet-land`, typically. 
    - e.g. `Hamby44-Barrel 1-Bullet 1-Land 1`, `Houston-Unknowns-Bullet 'K'-Land 1`
    - Note: for the Variability study, these need to include operator, machine, and round
4. `crosscut`: Numeric value of the crosscut used for manual groove ID. This should result from `x3p_crosscut_optimize`. 
5. `manual_code`: Code identifying who completed the manual identification  
    - e.g., "kr", "cr", "hh", "yg"
6. `manual_rep`: Repetition number within each individual's set of identifications.  
    - e.g. "kr" did 3 repetitions on Hamby Set 44, so there are reps 1, 2, and 3.
7. `groove_left_manual`: this is the manually identified groove on the left side of the crosscut (LEA). This should be a single number. 
8. `groove_right_manual`: this is the manually identified groove on the right side of the crosscut (LEA). This should be a single number. 


Please see `grooves_manual_hamby44.csv` for an example of what the data should look like, and match your format to that! 
