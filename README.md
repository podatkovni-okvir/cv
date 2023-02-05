# CV

Repo je nastao s ciljem izrade životopisa koji je lako ažurirati. Za izradu životopisa korišten je R, odnosno R Markdown.

Unosi se nalaze u googlesheetsu.
Publikacije se nalaze u .bib datoteci.
Kao dizajn je korišten `awesomecv` template iz R paketa `vitae`. 

Ukratko, podaci iz googlesheetsa i .bib datoteke provučeni su kroz funkcije iz paketa `vitae`
te u kombinaciji s pridavanjem pripadajućih naslova odjeljaka u .Rmd datoteci čine životopis.
U YAML zaglavlju se nalaze osnovne informacije poput imena, prezimena, kontakta i kratkog sažetka. 

-------
The purpose of this repo is to have a CV that is easily updatable. The code is writen in R, more precisely R Markdown. 

Entries are provided in a googlesheets document.
Publications are contained in a .bib file.
`awesomecv` template from R package `vitae` is used as a template. 

In short, data from googlesheets and .bib file is sent to the functions from `vitae` package, 
and in combination with provision of corresponding section titles in the .Rmd file, a CV is created.
Pieces of information such as name, surname, contact and a short "about me" section are contained in the YAML header. 


### Feel free to reuse: 
- clone repo
- change [.Rmd file](/bugarin_cv.Rmd) name (this determines the name of you .pdf output) 
- change [.bib file](data/publications-and-conferences.bib) (in case you do not want your resume to have publications, you can just delete that part of the code [starting at line 112])
- copy googlesheets document and change entries https://docs.google.com/spreadsheets/d/1_6JCugS2G_5Qr3eRJGMqKUubcg9WKMgGe2wlTDkxo2U/edit?usp=sharing 
- you can show or hide entries in your resume by putting "TRUE" or "FALSE" (respectively) in the column "show"
- change googlesheets URL in the [.Rmd file](/bugarin_cv.Rmd) [line 32] (your sheets need to be public)
- change resume section titles accordingly [starting at line 71] (delete the ones you do not want, add new ones; dataframes will have names that correspond to the section entries in googlesheets, eg. section "education" will be turned into "df_education" (if you want to have a detailed entry without bullet points, put "_" into column "description_1"))
- change YAML in the [.Rmd file](/bugarin_cv.Rmd) [first 15 lines] (here you can also have fun exploring different templates from the `vitae` package (if you do so, be aware of the code chunk at line 28 which alters highlight colors, might be best to delete it))

#### Resources:

`vitae` https://pkg.mitchelloharawild.com/vitae/reference/index.html - here you can read more about package functions and templates that it provides

If you are using R Markdown for the first time and you do not have LaTeX on your computer, you will need  
https://bookdown.org/yihui/rmarkdown-cookbook/install-latex.html  
or  
https://miktex.org/download


