# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read Class 02

### Testing and Modules

#### Test_Driven_Development

Unit tests are some pieces of code to exercise the input, the output and the behaviour of your code. You can write them anytime you want.

But Test-Driven Development is a strategy to think (and write!) tests first. With TDD we need to think about tests first.

Our test name need to be descriptive about the test,what is expected and what we are testing

The test file name should follow the same name of module name. like, giving a name test_snakes_cafe.py for a  module snakes_cafe.py.It is also best practice to separate the tests folder from the code

*A widely accepted convention in unit test is AAA:-*

__Arrange:__ organize the data needed to execute that piece of code (input)

__Act:__ execute the code being tested

__Assert:__ after executing the code,check if the result (output) is the same as expected

#### The Test-Driven_development Cycle

1. Write a unit test and make it fail. It needs to fail because the feature is NOT right

2. Write the feature and make the test pass

3. Refactor the code — the first version doesn’t need to be the beautiful.

#### Recursion

The process in which a function calls itself directly or indirectly is called recursion and the corresponding function is called as recursive function

Problems can be resolved easily by using recursive algorithm

A function is called direct recursive if it calls the same function. Example:-

        def directRecursive()

            code here

        directRecursive()

A function is called indirect recursive if it calls another function directly or indirectly. Example:-

        def indirectRecursive()

            code here

        indirectRecursiveTwo()

            code here

A recursive function is tail recursive *when recursive call is the last thing executed by the function* like the above direct recursive function example

































...............................................................................

__Attributions for the following Reference materials and their authors__

[In Test We Trust- TDD with Python by Ana Paula Gomes](https://code.likeagirl.io/in-tests-we-trust-tdd-with-python-af69f47e6932)


[Recursion](https://www.geeksforgeeks.org/recursion/)



[>> NEXT (Read: Class 03)](https://wondwosentsige.github.io/code-401-reading-note/class-03)