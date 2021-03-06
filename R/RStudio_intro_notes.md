# RStudio intro
RStudio is an open source interface for the R programming language.

## Material

### Location
Please create a folder called "RProjects" under "Documents"

### Rstudio Project

(2min)
Challenge 1 - New Rstudio Project
1. Click the "File" menu button (top left corner), then "New Project"
2. Click "New Directory"
3. Click "New Project" ("New empty project" if you have an older version of RStudio)
4. In Directory name type the name of your project, e.g. "RStudio_Intro" 
(Browse and select a folder where to locate your project, for example the RProjects folder)
5. Click the "Create Project" button

Projects make managing multiple directories straightforward. You can create an RPROJ file in a new directory or an existing directory that already has R code and data. You can also create the project file by cloning a version control repository, such as Git or Subversion.
.rproj stores information about our folder structure and the objects in the project (hence, manages history and rdata).

### Help

- help(functionname)
- functionname F1
- ?functionname 

### Creating a folder structure

- sessionInfo()
provides information about your platform, the versions of R and the packages that you are using and their versions
does anyone has something different? Why would that be?

- getwd()
- setwd()
- citation()
- ls()
- show folders and files with dir()
- list objects in the R environment with ls()
- a <- 12345667 
- remove objects from the environment rm(list = ls())
- list files again ls()

#### Working in pairs

Files:
  
  * Create file/folder dir.create("scripts")
  * visually create plots
  ** challenge create data and report folder **

  * file.create("scripts/cmds.R")
  
  * Create new documents Ctrl+Shift+N Cmd+Shift+N
  in the scripts folder, with the following names: test1.R, test2.R, test3.R
  
  * then delete the file with:  file.remove("scripts/test1.R") 
  
  * Delete file/folder
  * Rename file test2.R for mytest.R
  * Copy file test3.R
  * Change directory to data


### Shortcuts
arrows up and down
ctrl+ S
ctrl + Enter
home and end button
####
- Interrupt current command Esc Esc
- Run current line/selection Ctrl+Enter Cmd+Enter
- Find Ctrl+F
- Find in Files Ctrl+Shift+F Cmd+Shift+F
####
- Cut Ctrl+X Cmd+X
- Copy Ctrl+C Cmd+C
- Paste Ctrl+V Cmd+V
- Select All Ctrl+A Cmd+A
- Delete Line Ctrl+D Cmd+D
- Clear console Ctrl+l Cmd+l

- Indent Tab (at start of line) Tab (at start of line)
- Outdent Shift+Tab Shift+Tab

- Insert <- Alt+- Option+-
- Insert %>% Ctrl+Shift+M Cmd+Shift+M

- Move Lines Up/Down Alt+ up/down Option+up/down
- Copy Lines Up/Down Shift+Alt+up/down Cmd+Option+up/down

- (Un)Comment lines Ctrl+Shift+C Cmd+Shift+C

- See shortcuts Alt+Shift+K

#### Working in pairs - Layout 
Work in pairs 3min

Task Windows/Linux Mac

- Move focus to Source Editor Ctrl+1 Ctrl+1
- Move focus to Console Ctrl+2 Ctrl+2
- Move focus to Help Ctrl+3 Ctrl+3
- Show History Ctrl+4 Ctrl+4
- Show Files Ctrl+5 Ctrl+5
- Show Plots Ctrl+6 Ctrl+6
- Show Packages Ctrl+7 Ctrl+7
- Show Environment Ctrl+8 Ctrl+8
- Show Git/SVN Ctrl+9 Ctrl+9

Discuss with your peers
  
### Packages
install.packages("ggplot2")

### Import files  

download.file()
read.table()
read.csv()


    #!/usr/bin/env Rscript
    # Title: importing
    # Author: Paula A. Martinez
    # Date: 28/09/2017

    download.file(url = "https://raw.githubusercontent.com/orchid00/CDS/master/R/scripts/gapminder_example.R",
              destfile = "scripts/gapminder_example.R")
  
