# Welcome to Python

## Who am I
* Pete Alonzi
* PhD, physics
* Staff Data Scientist for the Data Science Institute
* From Chicago
* Selected hobbies: Sports, gaming, music

## Let's do something!
* logon to the rivanna portal: https://rivanna-portal.hpc.virginia.edu/pun/sys/dashboard/
* fire up a console like yesterday ``` Clusters --> >_Rivanna Shell Access ```
* type "python" then let's talk about what we see
* type ``` python ```
* what about python version 3?
* type ``` module load anaconda/5.2.0-py3.6 ```
* type ``` python ``` then let's talk about what we see
* **TAKEAWAY:** Be careful about python versions, keep an eye out as we go

# Goals for Today
1. Get python running (3 ways)
2. Get comfortable with python
3. Learn how to look up help

### A quick note
Today we are working on python. However there is some knowledge of programming that is required. Don't worry if you don't know it, please ask questions. I will do my best to answer them. And I will also do my best to indicate when something is a python specific detail and when it is a programming in general item.

## Getting Python "Anaconda" (this will take some time)
* [Windows](https://www.anaconda.com/download/#windows)
* [Mac](https://www.anaconda.com/download/#macos)
* terminology time
  * programming langugage vs software distribution
  * python2 vs python3

## A brief history
* Designed by [Guido van Rossum](https://www.google.com/search?q=google+image+search+guido+van+rossum&safe=off&rlz=1C5CHFA_enUS690US690&source=lnms&tbm=isch&sa=X&ved=0ahUKEwjE_eGK6KHdAhXrRd8KHUzBDHsQ_AUICigB&biw=1440&bih=697)
* version 1.0 1994
* version 2.0 2000
* version 3.0 2008 (not widely adopted until a few years ago)
* [logo](https://www.google.com/search?q=python+logo&safe=off&rlz=1C5CHFA_enUS690US690&source=lnms&tbm=isch&sa=X&ved=0ahUKEwi9xN-J8aHdAhVBMt8KHT-WDEEQ_AUICigB&biw=1440&bih=697)
* [anaconda logo](https://www.google.com/search?q=anaconda+logo&safe=off&rlz=1C5CHFA_enUS690US690&source=lnms&tbm=isch&sa=X&ved=0ahUKEwin88Gf8aHdAhUhiOAKHeGLBHYQ_AUICigB&biw=1440&bih=697)
* ![](https://gvanrossum.github.io/images/license.jpg)

## Anaconda Installation
* You must be careful! Let's step through the installation
* When you install you also register the application with the computer's package manager.
* For most you will run the file you downloaded. If not raise your hand.
* We are now going to install anaconda and then go on break once it is installed and opens.

# Break Break Break Break
* Pete will announce what time we resume.

## Spyder
* tour
  * text editor
  * variable explorer
  * console
  * control icons
* hotkeys
* [project details](https://docs.spyder-ide.org/projects.html)

## Outline
1. Strings and Functions
2. Data types
3. Loops
4. Logic
5. How to import (aka the most important part)

# Import (aka the most important part)
This is how you get code that other people have written. Without this ability no one would use python. We will use pandas as our example.

## Getting Pandas
Mothership: https://pandas.pydata.org/
* conda install pandas
* python3 -m pip install --upgrade pandas

To confirm installation:
* open python and type <pre>import pandas as pd</pre>

## Let's talk about pandas data frames

Definition of data frame:
* "Two-dimensional size-mutable, potentially heterogeneous tabular data structure with labeled axes (rows and columns). Arithmetic operations align on both row and column labels. Can be thought of as a dict-like container for Series objects. The primary pandas data structure." [official documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html)

### Often pandas data frames are confusing to new users. That is not the fault of the new user.

The trick is that pandas data frames have a lot of capability and many features. But when learning you don't need that. So today we'll focus on the fundamnetals.

* Working definition of Data Frame: 
    <pre> An allocation of computer memory that holds data, formatted like a spreadsheet.</pre>
* What a data fame "looks like"
    ![visualized](https://github.com/alonzi/pandas-intro/blob/master/andre.png) 
    



## Other Resources
* Python for Data Analysis by McKinney - [get from library](https://search.lib.virginia.edu/catalog/u7444998)
* R for Data Science by Wickham & Grolemund - [free online](https://r4ds.had.co.nz/)

# Project Jupyter
![The Third Heat](https://github.com/UVA-DSI/2019-bootcamp/blob/master/python3/thirdheat.jpg)

*The third heat.*


* projects/working directory/command line/essential toosl/c(...)/=/docs/indexing/data frames/plots/load data



# Homework
## Ways to Practice
1. Write some code (a game is often a good exercise, like tic tac toe)
2. Ask a friend to review it

* Beginning
  * Flip a coin (~10 lines)
  * Play rock, paper, scissors  (~25 lines)
* Intermediate
  * Guess a secret number between 1 and 10. With hints. (~20 lines)
  * Dice rolling program
* Expert
  * Play blackjack
  * Play roulette
