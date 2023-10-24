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
- formatting can be (largely) controlled by creating a word-styles-reference.docx file, as explained [here](https://rmarkdown.rstudio.com/articles_docx.html)
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

