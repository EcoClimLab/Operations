# Data creation practices
## ForestGEO Ecosystems & Climate Lab @ SCBI

Our lab’s (internal) master versions of most data sets are mananged and archived on GitHub. GitHub is used to track data versions, record what changes have been made, and back up old versions. It is also used to record communications about the data (“issues”).

## Data Format
For guidelines on formatting data sets, see [Nine simple ways to make it easier to (re)use your data](https://ojs.library.queensu.ca/index.php/IEE/article/view/4608).

## Procedures:
### Data entry
For individuals with expertise in the data set (research assistants, postdocs, etc.), data files may be produced and updated using any program. 

To facilitate data entry by individuals without expertise in the data set (practicum students, volunteers, etc.), we can create [Google spreadsheets](https://www.google.com/sheets/about/). Possible values for any field can be constrained. 

### Updating/ correcting data
When data are being added to an existing data sheet or new data are being added, the file to be modified is the current master on Github (see also the section on sharing/ collaborating outside the lab). 

Data updates should be saved frequently to a shared storage location (e.g., GitHub, Google spreadsheets, lab hard drive). At a minimum, this should happen at the end of each day during which data were modified.  

### Loading to Github
Once new or updated data sheets have been screened by someone with expertise in the data set, they are pushed to GitHub along with comments as to what data have been added/ what changes have been made. 

### Collaborations / Data sharing 
- When collaborating on data creation with researchers who do not use GitHub, there will be two versions of data (or code): master_shared and master_KATlab 
     - master_shared is the version that is shared with the other research group. This version may be housed in any file sharing system. It is understood that both research groups have their own internal processes and quality control procedures for updating this version. 
     - master_KATlab is the version that is managed according to our scientific workflow procedures. It is managed on GitHub. 
       - When we update the master, that update is recorded in Github, and we also copy the new master to master_shared. 
       - When the other research group updates the master, we load the new version to Github as a branch. It is then reconciled with and merged into master_KATlab. If changes are required, we record those on Github and update master_shared.
-	Ways to share Github information with non-GitHub users
      - For an entire repository
         - Make the repository public
          - Create a guest account, give password
        - Make a website for the repository. Read about Github pages [here](https://help.github.com/articles/configuring-a-publishing-source-for-github-pages/).
      - For a single folder within a private repository
         - Put Github repository in Dropbox, share just the desired folder
         - Move the folder to a separate repository
         - Create orphan branch with all private material deleted (so that it can’t be retrieved through history)
