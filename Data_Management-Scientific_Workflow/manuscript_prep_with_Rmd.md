# Manuscript prep with .Rmd

## Why .Rmd?
- .Rmd files integrate seemlessly with R and GitHub, allowing integration of code and version control/ reproducibility 
- .Rmd files can be opened / edited in Rstudio, and knit into HTML, PDF, or DOCX files with the push of a button.

## General how-to / introductory guides
- [Composing reproducible manuscripts using R Markdown](https://elifesciences.org/labs/cad57bcf/composing-reproducible-manuscripts-using-r-markdown)
- [Introduction to R Markdown](https://rmarkdown.rstudio.com/articles_intro.html)
- https://jhemberger.github.io/posts/posts/r-markdown-manuscripts/
- https://stirlingcodingclub.github.io/Manuscripts_in_Rmarkdown/Rmarkdown_notes.html
__________

## Output
- .Rmd can be knit to output .pdf, .docx, or .html.
- We use .docx most commonly, .pdf and .html for specialized purposes

### .docx

#### Advantages
- most journals require submissions (once accepted) in .docx
- easiest for sending to non-GitHub coauthors for feedback (as Word doc or Google doc)

#### Distadvantages
- some formatting can be tricky or occasionally impossible


#### Header content:
<img width="861" alt="image" src="https://github.com/EcoClimLab/Operations/assets/6355854/a5fe8947-4b10-4d55-b6c9-185199e2d111">

#### tips
- to control formatting, create a word-styles-reference.docx file, as explained [here](https://rmarkdown.rstudio.com/articles_docx.html)
- for tables, use R package [flextable](https://cran.r-project.org/web/packages/flextable/index.html) - [guide](https://ardata-fr.github.io/flextable-book/)


### .pdf
#### Advantages 
- more flexibility with some formatting:
  - tables - can use [kable and kableExtra](https://cran.r-project.org/web/packages/kableExtra/vignettes/awesome_table_in_html.html)
  - figures - easier to adjust size, position
  - direct formatting of headers, etc.
- .pdf output preferred for some purposes.
  
#### Disadvantages
- journals ultimately need word file
- hard to get edits from collaborators

#### tips
- for tables, use use [kable and kableExtra](https://cran.r-project.org/web/packages/kableExtra/vignettes/awesome_table_in_html.html)

## References
Need two files (both saved in same folder as .Rmd):
- Citations (.bib) file (can be automatically generated in zotero)
- Journal citation style (.csl) file : available for download in [this GitHub repository](https://github.com/citation-style-language/styles) or in the [Zotero style library](https://www.zotero.org/styles).

### software needed
- Zotero
  - need to download Better BibTex add-on for Zotero: https://retorque.re/zotero-better-bibtex/installation/

### generating the .bib file
#### step 1. set up Zotero preferences to generate a citation key
The goal is to generate a citation key as in this image (screenshot of Zotero):
<img width="449" alt="image" src="https://github.com/EcoClimLab/Operations/assets/6355854/808b18e7-1971-4ee6-b3db-6765b1a83a8f">


This can be adjusted in settings: 

![image](https://github.com/EcoClimLab/Operations/assets/6355854/cde8090e-c706-401d-999e-0ca8fdd0bf34)

Your citation key format can be whatever you want, but collaboration is easiest when citation key formats match. 
Here's Krista's citation key format: `auth.lower+"_"+veryshorttitle(1,1).lower+"_"+year`

#### step 2. generate the .bib file
I create a separate Zotero library for each manuscript/ project. 
One advantage of this is that you have a smaller library and it's easier to troubleshoot issues with the .bib file. 
It also allows sharing the library with collaborators (best when they have the same citation key format). 

To export, right-click on the relevant library and match the following images:

![image](https://github.com/EcoClimLab/Operations/assets/6355854/e5cab20e-b224-47a8-b80c-9b824cea8368)
![image](https://github.com/EcoClimLab/Operations/assets/6355854/9c63f7e1-8a05-4372-9cad-55dc838f4c00)

... Then save .bib file in the same directory as your .Rmd file.

### adding citations

To insert citation, simply copy the citation key and include after an "@". 
For example,
- [@friedlingstein_global_2022] --> (Friedlingsten et al. 2022)
- @friedlingstein_global_2022 --> Friedlingsten et al. (2022)
- [e.g., @friedlingstein_global_2022] --> (e.g., Friedlingsten et al. 2022)
- [Fig. 1, @friedlingstein_global_2022] --> (Fig. 1, Friedlingsten et al. 2022)

