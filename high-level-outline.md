# High Level Outline for 2019 DSI residential bootcamp

This document lists the high level points that will be covered in the DSI bootcamp. Each instructor will build out the details of their section.



## July 1, AM: Intro to computers for scientists
0. High Level questions to frame the program - not to answer today
  * When should I terminal/script/program/text editor/IDE?
  * When should I use R v Python?
  * Does this fit in memory/ Do I need more than my laptop?
  * It's ok to freeze and not know what to do, that means you are about to learn. Feel the burn
  * Which ml tool is  right for the job?
  * How  do I translate a research question into a data question? How to I translate a data answer to a research answer?
1. operating systems
2. the shell
  * Command Line Interface (CLI):
     1. We use the Bourne-again Shell (BASH)
     1. use sagemaker for unified terminal environment
     2. mkdir, cd, ls, history
     3. installation on student laptop is homework
  * GUI
3. version control (git/github)
5. text editor v word processor v IDE (eg: vi vs. VS Code vs. Rstudio)
6. grab bag
  * "#" is a comment in BASH,R,Python
9. Reading list:  
  * [bryan wright's stuff](http://galileo.phys.virginia.edu/compfac/courses/sysadmin1)
  * geek-hours/shell.html

## July 1, PM: R
0. History
1. RStudio and installation
  1. tour / hotkeys
  2. projects and working diretory
  3. commandline from inside RStudio
2. Base R essential tools
  1. c(...), functions how they work
  2. "anatomy of coding" aka syntax or grammar
  3. "?", "<-"
  4. indexing (start from 1)
  5. operators
3. Data Frames
  1. details
  2. getting data in
  3. manipulating
4. Simple Plots
5. Tidying up
6. ReadingList:  
  * [R for data science](https://r4ds.had.co.nz/) 

## July 2, AM: Python3
0. History
1. anaconda/spyder/jupyter
  1. tour and hotkeys
  2. working directory
  3. commandline from inside spyder
2. python 3 essentials
  1. int,float,string,lists
  2. indexing (start at 0)
  3. functions, "anatomy"
  4. assignment operator and a couple others
3. Data frames - import pandas as pd
4. simple plot
5. Load data into data frame
6. Reading List:  
  * [Python Data Science Handbook by VanderPlas](https://jakevdp.github.io/PythonDataScienceHandbook/)

## July 2, PM: Thinking like a data scientist (aka Putting it all togegther (aka the most fun part))
This is language agnostic. The prompt works for R and Python. We give examples in both languages.
The goal of this part is to open the world to how a data scientist operates and thinks.

1. reading in data -- dealing with .tsv files
2. Understanding a dataframe as observations and features
3. data types and coercing variables to proper format (text vs. categorical, etc.)
4. formatting dates
5. using the summary() function for information about variables and possible outliers (include use of hist here)
6. NAs and the absence of data -- discuss possible methods to handle, but for our purposes delete rows/columns with NAs
7. adding a column (feature engineering)
8. pairplots to study correlation and spot potentially interesting relationships.
9. plotting data
