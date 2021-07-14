# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Pandas

What Is Pandas In Python?

Pandas is an open source Python package that is most widely used for data science/data analysis and machine learning tasks. It is built on top of another package named Numpy, which provides support for multi-dimensional arrays.

Pandas makes it simple to do many of the time consuming, repetitive tasks associated with working with data, including:

    Data cleansing
    Data fill
    Data normalization
    Merges and joins
    Data visualization
    Statistical analysis
    Data inspection
    Loading and saving data
    And much more

We import pandas as follows

    In [1]: import numpy as np

    In [2]: import pandas as pd

The most elementary functions of panda are

    Reading data

        data = pd.read_csv('my_file.csv')

    Writing Data

        data = pd.read_csv('my_file.csv', sep=';', encoding='latin-1', nrows=1000, skiprows=[2,5]) 
        
        -----> index=None will simply write the data as it is. If you don’t write index=None, you’ll get an additional first column of 1,2,3, … until the last row.

    Checking the data

        data.shape  ----------------> Gives #rows, #columns

        data.describe() ------------> Computes basic ststistics
    
    Seeing the data

        data.head(3) ------------> Print the first 3 rows of the data. Similarly to .head(), .tail() will look at the last rows of the data.

        data.loc[8] ............> Print the 8th row

        data.loc[8, 'column_1'] ------> Print the value of the 8th row on “column_1”

        data.loc[range(4,6)] --------> Subset from row 4 to 6 (excluded)

[10 minutes in pandas](https://pandas.pydata.org/pandas-docs/stable/user_guide/10min.html)

[Getting started tutorials](https://pandas.pydata.org/pandas-docs/stable/getting_started/intro_tutorials/index.html)

[Pandas for data science](https://realpython.com/learning-paths/pandas-data-science/)

[Master pandas](https://towardsdatascience.com/be-a-more-efficient-data-scientist-today-master-pandas-with-this-guide-ea362d27386)




















...............................................................................

__Attributions for the following Reference materials and their authors__

[What is Pandas in Python?](https://www.activestate.com/resources/quick-reads/what-is-pandas-in-python-everything-you-need-to-know/)

[What is Pandas in Python? Youtube video](https://www.youtube.com/watch?v=dcqPhpY7tWk&t=391s)



[>> NEXT (Read: Class 13)](https://wondwosentsige.github.io/code-401-reading-note/class-13)
