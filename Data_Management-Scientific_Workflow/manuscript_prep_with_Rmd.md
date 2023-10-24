# Manuscript prep with .Rmd

## Why .Rmd?
- [Composing reproducible manuscripts using R Markdown](https://elifesciences.org/labs/cad57bcf/composing-reproducible-manuscripts-using-r-markdown)

## How-to guides
- [Introduction to R Markdown](https://rmarkdown.rstudio.com/articles_intro.html)
- https://jhemberger.github.io/posts/posts/r-markdown-manuscripts/
- https://stirlingcodingclub.github.io/Manuscripts_in_Rmarkdown/Rmarkdown_notes.html

## Output
- .Rmd can be knit to output .pdf, .docx, or .html.
- We use .docx most of the time, .pdf or .html for some specialized purposes

### .docx
#### Advantages
- most journals require submissions in .docx
- easiest for sending to non-GitHub coauthors for feedback

#### Distadvantages
- some formatting can be trickier


### .pdf
#### Advantages 
- more flexibility with some formatting:
  - tables - can use [kable and kableExtra](https://cran.r-project.org/web/packages/kableExtra/vignettes/awesome_table_in_html.html))
  - figures - easier to adjust size, position
  - direct formatting of headers, etc.
- .pdf output preferred for some purposes.
  
#### Disadvantages
- journals ultimately need word file
- hard to get coauthor feedback
