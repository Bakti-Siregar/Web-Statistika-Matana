# Web Statistika ~ Matana University

This repository created for Department of Statistics ~ Matana University, Tengerang, Indonesia. Please feel free to follow alone step by step of building a Website using R Blogdown bellow:

## Install R and Rstudio
## Install Git
## GitHub Account 
* New Repository > Readme> Licence> master branch 
* Get the link of your `https://github.com/your_user_name/your_repository_name.git` 

## Open your RStudio 
* Click Tools > Global Options > Git/SVN > C:/Program Files/Git/bin/git.exe > Apply > Ok
* File > New Project > Version Control > Git 
* Repository URL: https://github.com/your_user_name/your_repository_name.git, *Ex:* `https://github.com/Bakti-Siregar/Web-Statistika-Matana.git`
* Project Direcory Name : the default should be `your_repository_name`, *Ex:* `Web-Statistika-Matana`. Feel free change it if you want to
* Subdirectory: Depends on You, choose anywehere you want.
* Click `Create Project`

## Install Some packages 

* `install.packages("devtools")`
* `install.packages("blogdown")` 
* `blogdown::install_hugo()`

## Select Hugo Theme 
* Here I select : https://themes.gohugo.io/toha/
* Go to https://github.com/hossainemruz/toha
* Back to your RStudio Console and type: `blogdown::new_site(theme="themefisher/educenter-hugo")`

## Stop the default Server
* servr::daemon_stop(1)

## Setting GitHub Config
* Go to: Tools > Sheell...
* Copy, paste, and Enter : `git config --global user.name "Bakti-Siregar"`
* Copy, paste, and Enter : `git config --global user.email "siregarbakti@gmail.com"`
* Copy, paste, and Enter : `git add -A`
  
## Commit to GitHub
* Git > Commit > Select All > Type your Coomit massege > Commit > Push 

## Netlify Account 
* Sign UP 
* Log In with your Github Account 
* Go to : New Side from GitHub > `your_repository_name` > Show advanced > New variable
* Type in Key: `HUGO_VERSION` 
* Type in Value: The latest Hugo version is `0.75.1` , you can check it in RStudio : `blogdown::hugo_version()`
* Deploy Site 


