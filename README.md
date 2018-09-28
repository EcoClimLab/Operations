# Data Management & Scientific Workflow

## ForestGEO Ecosystems & Climate Lab @ SCBI

This repository is focused on the lab's scientific workflow and data management, including procedures and resources. 

## About these guidelines
These guidelines are informed by best (or ["good enough"](https://doi.org/10.1371/journal.pcbi.1005510)) practices guidance for scientific workflow and data management and adjusted to fit the needs of our lab. They are not intended as strict rules (especially when it comes to details), but are designed to ensure good practices and consistency throughout the lab. 

Researchers in the lab are expected to be familiar with lab procedures (outlined here) and ensure that their practices are compatible with these procedures. Researchers who are not yet very experienced with data management and best practices in scientific workflow are asked to follow these guidelines closely, and should view implementation of these practices as a learning opportunity that will benefit their future scientific careers. Those with more experience may have more leeway to follow their own system, providing that they use solid scientific workflow/ data management practices that can be integrated with lab practices. Researchers in the lab should develop plans for data management and scientific workflow in conjunction with their mentor at the beginning of each project. 

Not all projects are currently up to speed with these guidelines, but we are striving to adopt these procedures with all new projects and to bring ongiong projects up to speed. 

This is a working document, and lab procedures are subject to change. Lab members and collaborators are encouraged to provide feedback and ideas to help improve practices. 


## Open access policy
Scientific data and code are valuable resources that we wish to preserve indefinitely, long beyond the lifespan of a project or even the researchers involved. Policies of the U.S. government, the Smithsonian, funding agencies, and most journals require that scientific data be made publicly available in a timely manner. Moreover, ensuring preservation of work effort and reproducibility of results requires public archiving of code. Our lab strives to follow best practices so as to ensure the long-term value of our data and code. **All researchers should work under the expectation that all data and code will be made public**, either immediately or upon publication of the first manuscript using them.


## Workflow overview
- Scientific workflow is grouped into “projects”. A project is typically creation of a data set (which may be used in multiple publications) and/or an individual publication (which may draw upon multiple data sets).
- Data work is separated into distinct (but often closely integrated) phases:
  - [Data creation](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/tree/master)- This phase consists of collecting, entering, and checking data. Data creators are responsible to correct data errors/ provide updated versions.
  - [Data analysis](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/blob/master/data_creation.MD)- This phase consists of preparing code to analyze raw data files. Data analysts do not change the original files – everything goes in the script. Ideally, all data processing is automated, such that script can generate figures and tables for publication by running a single script. 
  - [Publication/ Presentation](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/blob/master/publication_presentation.MD)- This phase consists of preparing publications or presentations. 
- Each project typically has shared materials managed in 2-3 locations:
  - GitHub: data, code, and results. Access to the Github repository will be given to lab members and external collaborators working on data production and analysis. GitHub is also used to manage scientific workflow/ track "issues". 
    - Note that GitHub + RStudio can provide a great environment for preparing publications, but for now most projects will use Word/ sharing in Dropbox. 
  - Dropbox: manuscript, references, other supporting documents. Dropbox facilitates sharing with all collaborators (not just those using GitHub). 
  - SCBI's file server: large files, such as images (e.g., scans of leaves or tree cores), map data, massive data sets
 


## For new lab members
1. Please review the documents in this repository
2. Discuss research/ data management plans with your mentor
3. Get oriented with the [tools](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/blob/master/tools.md) that are vital to our scientific workflow. If necessary, install, create accounts, and teach yourself the basics of how to use these. 

## Useful references:
- Wilson G, Bryan J, Cranston K, Kitzes J, Nederbragt L, Teal TK (2017) [Good enough practices in scientific computing](https://doi.org/10.1371/journal.pcbi.1005510). PLoS Comput Biol 13(6): e1005510.
