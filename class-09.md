# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Dunder Methods

In Python, special methods called __dunder methods__ are a set of predefined methods you can use to enrich your classes. They are easy to recognize because they start and end with double underscores.

Dunder methods let you emulate the behavior of built-in types

To construct objects from a class we need a constructor which in Python is the __init__ dunder:

The “official” string representation of an object is __repr__ dunder. This is how you would make an object of the class. The goal of __repr__ is to be unambiguous.

The “informal” or nicely printable string representation of an object is the __str__ dunder. This is for the end user.

In order to iterate over our object in python, we need __len__, __getitem__, and __reversed__ dunders

We can make an object callable like a regular function by adding the __call__ dunder method

## Statistics - Probability

At the most basic level, probability seeks to answer the question, “What is the chance of an event happening?”

An event is some outcome of interest. To calculate the chance of an event happening, we also need to consider all the other events that can occur.

To calculate the probability of an event occurring, we count how many times are event of interest can occur (say flipping heads) and dividing it by the sample space.

In a coin toss the only events that can happen are:

    flipping a heads

    flipping a tails

An ideal coin will have a 1-in-2 chance of being heads or tails











...............................................................................

__Attributions for the following Reference materials and their authors__

[Enriching Your Python Classes With Dunder (Magic, Special) Methods - Bob Belderbos](https://dbader.org/blog/python-dunder-methods)

[Tutorial: Basic Statistics in Python — Probability - DATAQUEST](https://www.dataquest.io/blog/basic-statistics-in-python-probability/)

[>> NEXT (Read: Class 10)](https://wondwosentsige.github.io/code-401-reading-note/class-10)
