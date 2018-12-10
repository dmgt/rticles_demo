# rticles_demo
**Example of creating PDFs in journal-specific formats from RMarkdown templates provided with the [`rticles`](https://github.com/rstudio/rticles) package from Rstudio**

[Here](https://daijiang.name/en/2017/04/05/writing-academic-papers-with-rmarkdown/) is an additional paper template written in RMarkdown by Dr. Daijiang Li

**How to use this repo:**
 - After following the setup instructions [here](https://github.com/rstudio/rticles) and if neccesary the additional troubleshooting in `notes.Rmd`below, open an .Rmd file from one of the test directories and click knit (in RStudio GUI above) to output a PDF formatted for a specific journal
 
 - More recently added journal tmeplates (eg Springer) were not installed with `rticles` but are avalible on  https://github.com/rstudio/rticles


**This repository contains:**

- `notes.Rmd` - instructions on one way of installing `rticles` and configuring it with MiKTeX on Windows 10.
    - .`Renviron` is one of the files created by this setup  
    
    
- *plos_test* - repository containing an RMarkdown template, associated files, and a PDF file created from the .Rmd file. 
    - The files automatically created for the *PLOS* template from `rticles` are below. In general you won't have to worry about editing these files by hand, but don't delete them either since some are required for the .Rmd --> .md --> .TeX --> .pdf conversion to work correctly.  
    
        - plos_test.Rmd - the main RMarkdown file to be knit
        - PLOS-submission.eps - this is the logo
        - PLOS-submission-eps-converted-to.pdf - logo in pdf format
        - mybibfile.bib - this is where the references go
        - plos.csl 
        
        
    - The output files of knitting the .Rmd file are:
        - plos_test.tex
        - plos_test.pdf

            
- *elsevier_test* - repository containing an RMarkdown template, associated files, and a PDF file created from the .Rmd file. 
    - The files automatically created for the *Elsevier* template from `rticles` are below. In general you also won't have to worry about editing these files by hand, but some are required for the .Rmd --> .md --> .TeX --> .pdf conversion to work correctly. 
    
        - elsevier_test.Rmd - the main RMarkdown file to be knit
        - skeleton.tex - example included with repo
        - skeleton.pdf - example included with repo
        - numcompress.sty
        - mybibfile.bib - this is where the references go
        - elsearticle.cls 

    - The output files of knitting the .Rmd file are:
        - elsevier_test.tex
        - elsevier_test.pdf
        - elsevier_test.spl (Windows spool file?)

    

