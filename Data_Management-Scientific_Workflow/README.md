# Data Management & Scientific Workflow

## ForestGEO Ecosystems & Climate Lab @ NZCBI

This repository is focused on the lab's scientific workflow and data management, including procedures and resources. 

## About these guidelines
These guidelines are informed by best (or ["good enough"](https://doi.org/10.1371/journal.pcbi.1005510)) practices guidance for scientific workflow and data management and adjusted to fit the needs of our lab. They are not intended as strict rules, but are designed to ensure good practices and consistency throughout the lab. 

Researchers who are not yet very experienced with data management and best practices in scientific workflow are asked to follow these guidelines, and should view implementation of these practices as a learning opportunity that will benefit their future scientific careers. Those with more experience have more leeway to follow their own system, providing that they use solid scientific workflow/ data management practices that can be integrated with lab practices as needed. 

This is a working document. Lab members and collaborators are encouraged to provide feedback and ideas to help improve practices. 


## Open access policy
Scientific data and code are valuable resources that we wish to preserve indefinitely, long beyond the lifespan of a project or even the researchers involved. Policies of the U.S. government, the Smithsonian, funding agencies, and most journals require that scientific data be made publicly available in a timely manner. Moreover, ensuring preservation of work effort and reproducibility of results requires public archiving of code. Our lab strives to follow best practices so as to ensure the long-term value of our data and code. **All researchers should work under the expectation that all data and code will be made public**, either immediately or upon publication of the first manuscript using them.


## Workflow overview
- Scientific workflow is grouped into “projects”. A project is typically creation of a data set (which may be used in multiple publications) and/or an individual publication (which may draw upon multiple data sets).
- Data work is separated into distinct (but often closely integrated) phases:
  - [Data creation](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/blob/master/data_creation.MD)- This phase consists of collecting, entering, and checking data. Data creators are responsible to correct data errors/ provide updated versions.
  - [Data analysis](https://github.com/EcoClimLab/Data_Management-Scientific_Workflow/blob/master/data_analysis.MD)- This phase consists of preparing code to analyze raw data files. Data analysts do not change the original files – everything goes in the script. Ideally, all data processing is automated, such that script can generate figures and tables for publication by running a single script. 
  - Publication/ Presentation - This phase consists of preparing publications or presentations. This can be done within or outside of GitHub. We use [R Markdown in GitHub](https://github.com/EcoClimLab/Operations/blob/master/Data_Management-Scientific_Workflow/manuscript_prep_with_Rmd.md) to prepare most publications.
- Each project typically has shared materials managed in  locations:
  - GitHub: data, code, results, manuscripts, and other supporting documents. Access to the Github repository will be given to lab members and external collaborators working on data production and analysis. GitHub is also used to manage scientific workflow/ track "issues".
  - shared Zotero libraries with references
  - NZCBI's file server: large files, such as images (e.g., scans of leaves or tree cores), map data, massive data sets


## Useful references:
- Wilson G, Bryan J, Cranston K, Kitzes J, Nederbragt L, Teal TK (2017) [Good enough practices in scientific computing](https://doi.org/10.1371/journal.pcbi.1005510). PLoS Comput Biol 13(6): e1005510.
- White et al. (2013). [Nine simple ways to make it easier to (re)use your data ](https://ojs.library.queensu.ca/index.php/IEE/article/view/4608). Ideas in Ecology and Evolution.
