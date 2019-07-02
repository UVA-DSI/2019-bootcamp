# Reading in Data
Our first step is to read data into a pandas data frame. It may be coming from many diferent sources (Eg: a file in storage, an object in memory, the internet, etc.). Here we will look at the example of reading in from a file (.csv).
 
  * read from csv files
    * docs: https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.read_csv.html
      
      don't worry if this looks intimidating, we'll break it down
  * Let's write a program
    <pre>
    # load pandas package
    import pandas as pd
    </pre>
    <pre>
    # read data into data frame
    df =  pd.read_csv("andre.csv")
    </pre>
    
# Manipulating Data

### Taking a look at the data
Your data in a data frame is stored in memory. But as a human we like to see a snippet on the screen. Let's write a program to do just that.

    # load pandas package
    df.head()
    
    # look at end of file
    df.tail()
    
    # look at random sample
    n = 5
    df.sample(n)

* Notice how the whole frame doesn't display. If you want to see the column names you can do this:
<pre>
list(df)
</pre>

### Sort
In this world we call sorting the data set on a column "arranging". To write aprogram to do that we use the function 'sort_values'.
  * [documentation](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.sort_values.html)

  <pre>df.sort_values(by='G', ascending=False)</pre>
    
### Remove rows (with condition)
Sometimes we want to remove some of the data. We call that filtering. Let's try writing code to remove the years before 1976 from this data frame.

<pre>
df = df[ df.Year > 1976 ]
</pre>

Code Breakdown:
* df is a data frame object
* the " [ ... ] " let's us reference or "index" the data frame
* df.Year > 1976 is a boolean that is evaluated for every row



### Create or Remove Columns
* Once you have worked the data set you sometimes want to select a subset of the columns going forward. Again we use the reference tool and provide a list of columns to keep.

    <pre>
    df = df[ ['H','G'] ]
    </pre>


* To create columns we can even get a little fancier and stick calculations right into those new columns.
mutate (aka create new columns). Let's make up batting average.

    <pre>
    df['myBA']=df.H/df.AB
    df[['myBA','BA']]
    </pre>

  To create the new column we just acted like it existed and pandas created it for us on the fly.


# Aggregation / summarization

* To quickly summarize the common statistics of the dataset use describe
  <pre> df.describe() </pre>

* There are also a bunch of pandas functions to do some stats and things
  * df.mean()
  * << google practice time >>

* pandas also facilitates group operations. To explain let's look at a picture.
-- show picture on your desktop from the pandas book because it is not open source.
  * let's group Andre's data frame by Team he played for then take the mean
 <pre>dfg = df.groupby(df.Tm)</pre>
 <pre>dfg.mean()['H']</pre>


# Making plots
Let's make a histogram from our sample dataset. Since we are using a data frame this feature is already built in

<pre>
# make a histogram
df.hist("H",bins=100)
</pre>

![](https://github.com/alonzi/pandas-intro/blob/master/histo.png)

