# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## JupyterLab

JupyterLab is a next-generation web-based user interface for Project Jupyter.

It enable us to work with documents and activities such as Jupyter notebooks, text editors, terminals, and custom components in a flexible, integrated, and extensible manner

## NumPy Tutorial: Data Analysis with Python

**NumPy** _is a commonly used Python data analysis package_. By using NumPy, you can speed up your workflow, and interface with other packages in the Python ecosystem, like scikit-learn, that use NumPy under the hood

 A __2-dimensional array is known as a matrix__, a matrix has rows and columns. By specifying a row number and a column number, we’re able to extract an element from a matrix.

 In a NumPy array, *the number of dimensions is called the rank, and each dimension is called an axis*. So the rows are the first axis, and the columns are the second axis.

*We can create a NumPy array using the numpy.array function*. If we pass in a list of lists, it will automatically create a NumPy array with the same number of rows and columns.

One of the limitations of NumPy is that all the elements in an array have to be of the same type

We can check the number of rows and columns in our data using the **shape** property of NumPy arrays

Another methods that we can use to create NumPy arrays is to create an array where every element is zero. The below code will create an array with 3 rows and 4 columns, where every element is 0, using numpy.zeros:

    import numpy as np

    empty_array = np.zeros((3,4))

    empty_array

It’s useful to create an array with all zero elements in cases when you need an array of fixed size, but don’t have any values for it yet.























...............................................................................

__Attributions for the following Reference materials and their authors__

[Numpy tutorial:Data analysis with python - DATAQUEST](https://www.dataquest.io/blog/numpy-tutorial-python/)


[>> NEXT (Read: Class 12)](https://wondwosentsige.github.io/code-401-reading-note/class-12)
