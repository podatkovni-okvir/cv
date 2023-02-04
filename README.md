# cv

Repo je nastao s ciljem izrade životopisa koji je lako ažurirati. 

Unosi se nalaze u googlesheetsu.
Publikacije se nalaze u .bib datoteci.
Kao dizajn je korišten `awesomecv` template iz R paketa `vitae`. 

Ukratko, podaci iz googlesheetsa i .bib datoteke provučeni su kroz funkcije iz paketa `vitae`
te u kombinaciji s pridavanjem pripadajućih naslova odjeljaka u .Rmd datoteci čine životopis.
U YAML zaglavlju se nalaze osnovne informacije poput imena, prezimena, kontaka i kratkog sažetka. 

-------
The purpose of this repo is to have a CV that is easily updatable.

Enteries are provided in a googlesheets document.
Publications are contained in a .bib file.
`awesomecv` template from R package `vitae` is used as a template. 

In short, data from googlesheets and .bib file is sent to functions from the `vitae` package, 
and in combination with provision of corresponding titles in the .Rmd file creates a CV.
Information like name, surname, contact and short "about me" section is contained in the YAML header. 
