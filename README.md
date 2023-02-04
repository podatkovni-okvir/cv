# CV

Repo je nastao s ciljem izrade životopisa koji je lako ažurirati. 

Unosi se nalaze u googlesheetsu.
Publikacije se nalaze u .bib datoteci.
Kao dizajn je korišten `awesomecv` template iz R paketa `vitae`. 

Ukratko, podaci iz googlesheetsa i .bib datoteke provučeni su kroz funkcije iz paketa `vitae`
te u kombinaciji s pridavanjem pripadajućih naslova odjeljaka u .Rmd datoteci čine životopis.
U YAML zaglavlju se nalaze osnovne informacije poput imena, prezimena, kontakta i kratkog sažetka. 

-------
The purpose of this repo is to have a CV that is easily updatable.

Entries are provided in a googlesheets document.
Publications are contained in a .bib file.
`awesomecv` template from R package `vitae` is used as a template. 

In short, data from googlesheets and .bib file is sent to functions from the `vitae` package, 
and in combination with provision of corresponding section titles in the .Rmd file creates a CV.
Pieces of information such as name, surname, contact and short "about me" section are contained in the YAML header. 


## Feel free to reuse: 
- clone repo
- change .Rmd file name (this determines the name of you .pdf output) 
- change YAML in the [.Rmd file](/bugarin_cv.Rmd) [first 15 lines] (here you can also have fun exploring different templates from the `vitae` package (be careful of the code chunk at line 28 which alters highlight colors, might be best to comment it (crtl + shift + c)))
- copy googlesheets document and change entries https://docs.google.com/spreadsheets/d/1_6JCugS2G_5Qr3eRJGMqKUubcg9WKMgGe2wlTDkxo2U/edit?usp=sharing 
- change googlesheets URL in the code [line 32] (your sheets need to be public)
- change resume section titles accordingly (delete the ones you do not want, add new ones; dataframes will have names that correspond to the section entries in googlesheets, eg. section "education" will be turned into "df_education" (if you want to have a detailed entry without bullet points, put "_" into column "description_1"))
- change [.bib file](/data/publication-and-conferences.bib) (in case you do not want your resume to have publications just delete or comment that part of the code [starting at line 112])


`vitae` https://pkg.mitchelloharawild.com/vitae/reference/index.html
