# Data analysis guidelines
## ForestGEO Ecosystems & Climate Lab @ SCBI

## Overview
- Github is used to manage data analysis code and products (results and any intermediary data sets). It is also used to record communications about the analysis (“issues”). 
- Data analysis is organized by project. Some projects may share the same data and code, but each project should be stand-alone.
## Procedures:
  - **Raw data:** Data analysis starts with data file(s) passed from the data creation step or from a collaborator. 
      - These original files are preserved exactly as is (not even renamed), and should be accompanied by information on where they were obtained and any restrictions/ conditions on use.
      - Even for data produced within our lab, best practice is to keep a separate copy of the data file for analysis. This is so that (1) updates to the data file don’t break the code, (2) analyses can always be exactly reproduced 
      - These files should be read-only (at least in practice, may also change file permisisons).
  - **Intermediary data products:** If data require intermediary processing to be useful for analysis, and if this processing step is not fast or hard to automate, an intermediary data product may be stored. 
      - Best practice is that the process of getting from raw data to this intermediary data product be fully automated.
      - If full automation of this process is extremely time consuming or the analyst cannot figure out how to automate it, manual transformation may be considered. Consideration of this option should weight the possibility that the original data file will be updated—perhaps multiple times—requiring that the manual step be repeated. If any manual transformations are done, they must be thoroughly documented so that they can be exactly repeated.
      - Intermediary data products should not be manually modified (including renaming)!
  - **Code:** Ideally, all data processing is automated, such that script can generate figures and tables for publication by running a single script.
      - Code should be well-documented so that it is understandable to others and your future self. 
      - Write code with the  expectation that it will eventually be made public. That is, keep it clean and well-documented as you go.
      - Github will save code versions, so do not be afraid to delete parts that are no longer necessary.
      - Script organization
        - remove everything from the R environment: rm(list=ls())
        - force “random” numbers to be always the same, set.seed
        - define the (absolute) paths to data, scripts and results directories
        - load functionality: library, require, source
        - load data
        - review and clean data
        - do interesting things with the data
        - store results
  - **Results:** Production of figures and tables for publication should be fully automated
      - Script should output tables as they will appear in the manuscript, requiring at most copying and pasting into a formatted template. This will save repeated manual modification of tables in manuscripts.
      - Script should produce fully formatted figures that do not require modification for publication. (If full automation of this process is extremely time consuming or the analyst cannot figure out how to automate it, manual transformation may be considered. Consideration of this option should weight the possibility that the original data file will be updated—perhaps multiple times—requiring that the manual step be repeated.)
      
## Organization
- Data analysis may be organized as an R package using the template provided here: https://github.com/forestgeo/pkg 
- Github folder contents & naming conventions (idealized. No need to rename/restructure existing repositories that follow similar structure) 
  - README file – describes project, names accompanying Dropbox folder
  - Data: ‘data’ – if intermediary data product exists, rename
     - ‘raw_data’ – data files on
        - Accompanying README file should describe source/ conditions of use
     - ‘processed_data’- intermediary data products
  - Code: ‘scripts’ / 'src'
   - May contain sub-folders if necessary
  - Results: ‘results’ or ‘output’
