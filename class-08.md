# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## List Comprehensions in Python

List comprehensions provide a concise way to create lists.

It consists of brackets containing an expression followed by a for clause, then zero or more for or if clauses. The expressions can be anything, meaning you can put in all kinds of objects in lists.

The result will be a new list resulting from evaluating the expression in the context of the for and if clauses which follow it.

The list comprehension always returns a result list.

Create a simple list

    x = [i for i in range(10)]
    print x                     outputs -------> [0,1,2,3,4,5,6,7,8,9]

Create a list using loops and list comprehension

    For the next example, assume we want to create a list of squares. Start with an empty list

    # We can either use loops:

    squares = []

    for x in range(10):
        squares.append(x**2)
    print squares               outputs ----------> [0,1,4,9,16,25,36,49,64,81]


    # Or we can use lists comprehensions to get the same result:

    squares = [x**2 for x in range(10)]
    print squares                       outputs ----------> [0,1,4,9,16,25,36,49,64,81]

    JUST REMEMBER THE SYNTAX: [ expression for item in list if conditional ]

Multiplying parts of a list

Multiply every part of a list by three and assign it to a new list.

    list = [3,4,5]
    multiplied = [items*3 for item in list]

    print multiplied                        outputs -------> [9,12,15]

Show the first letter of each word

We will take the first letter of each word and make a list out of it.

    list_of_words = ["this", "is", "a", "list", "of","words"]

    items = [ word[0] for word in list_of_words ]

    print items                                  output ---------> ["t","i","a","l","o","w"]

Lower/Upper case converter

Let’s show how easy you can convert lower case / upper case letters.

    [x.lower() for x in ["A","B","C"]]      outputs ---------> ["a","b","c"]

    [x.upper() for x in ["a","b","c"]]      outputs ---------> ["A","B","C"]

Print numbers only from a given string

This example show how to extract all the numbers from a string.

    string = "Hello 12345 World"
    numbers = [x for x in string if x.isdigit()]
    print numbers                                   outputs -------->["1","2","3","4","5"]


...............................................................................

__Attributions for the following Reference materials and their authors__

[Linked Lists](https://www.pythonforbeginners.com/basics/list-comprehensions-in-python)


[>> NEXT (Read: Class 09)](https://wondwosentsige.github.io/code-401-reading-note/class-09)
