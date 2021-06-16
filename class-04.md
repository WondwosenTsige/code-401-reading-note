# Read Class 04

### Classes and objects

Objects are an encapsulation of variables and functions into a single entity.

Objects get their variables and functions from classes.

[Classes and objects: learnpython.org](https://www.learnpython.org/en/Classes_and_Objects)

I read the tutorial and did the exercise

### Think Recursively

to be done soon.

### pytest fixtures and coverage


#### Fixtures

when we have some objects available to all of our tests in which they might contain data we want to share across tests, or they might involve the network or filesystem. These are called "fixtures" in the testing world, and they take a variety of different forms.

In pytest, we define fixtures using a combination of the *pytest.fixture* decorator, along with a function definition.

Fixture can be helpful to provide our test an appropraite object rather than defining global variables.

I need to refer additional materials here

### Coverage

Code coverage is a way of checking that our test have run all of the code intended to test.

To include code coverage there's a package called pytest-cov on PyPI that you can download and install.

Once that's done, we can invoke pytest with the --cov option. like:

    pytest --cov

The document I am refering strongly suggest you provide an argument to --cov

Once it is done, we need to turn the coverage report into human readable format. suggested is HTML

    coverage html


...............................................................................

__Attributions for the following Reference materials and their authors__

[Classes and Objects: learnpython.org](https://www.learnpython.org/en/Classes_and_Objects)


[Python Testing with pytest: Fixtures and Coverage:- by Reuven M. Lerner](https://www.linuxjournal.com/content/python-testing-pytest-fixtures-and-coverage)



[>> NEXT (Read: Class 05)](https://wondwosentsige.github.io/code-401-reading-note/class-05)












