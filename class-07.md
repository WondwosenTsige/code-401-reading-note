# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Python Scope & the LEGB Rule: Resilving Names in Your Code

The concept of **scope** rules how variables and names are looked up in your code. It determines the visibility of a variable within the code. The scope of a name or variable depends on the place in which you created that variable in your code. *The Python scope concept is generally presented using a rule known as the LEGB rule which stands for stand for __Local, Enclosing, Global, and Built-in scopes*__.

Most commonly two general scopes are:

    1. Global scope: The names that you define in this scope are available to all your code.

    2.Local scope: The names that you define in this scope are only available or visible to the code within the scope.

only having global scoped names, any part of the program could modify any variable at any time, so maintaining and debugging large programs could become a real nightmare

Since Python is a dynamically-typed language, *variables in Python come into existence when you first assign them a value. On the other hand, functions and classes are available after you define them using def or class, respectively, anf modules exist after we import them*

I NEED TO READ and REFER more on dictionaries here.....(not clear)

*Local (or function) scope* is the code block or body of any Python function or lambda expression. This Python scope contains the names that you define inside the function. These names will only be visible from the code of the function. It’s created at function call, not at function definition, so you’ll have as many different local scopes as function calls. This is true even if you call the same function multiple times, or recursively. Each call will result in a new local scope being created.

*Enclosing (or nonlocal) scope* is a special scope that only exists for nested functions. If the local scope is an inner or nested function, then the enclosing scope is the scope of the outer or enclosing function. This scope contains the names that you define in the enclosing function. The names in the enclosing scope are visible from the code of the inner and enclosing functions.

*Global (or module) scope* is the top-most scope in a Python program, script, or module. This Python scope contains all of the names that you define at the top level of a program or a module. Names in this Python scope are visible from everywhere in your code.

*Built-in scope* is a special Python scope that’s created or loaded whenever you run a script or open an interactive session. This scope contains names such as keywords, functions, exceptions, and other attributes that are built into Python. Names in this Python scope are also available from everywhere in your code. It’s automatically loaded by Python when you run a program or script.

Enclosing or nonlocal scope is observed when you nest functions inside other functions. It takes the form of the local scope of any enclosing function’s local scopes.

Names defined in the enclosing Python scope are commonly known as *nonlocal names.*

Whenever we assign a value to a name in Python, one of two things can happen:

    1. we create a new name
    2. we update an existing name

*Modifying global names is generally considered bad programming practice because it can lead to code that is:*

    - Difficult to debug: Almost any statement in the program can change the value of a global name.

    - Hard to understand: You need to be aware of all the statements that access and modify global names.

    - Impossible to reuse: The code is dependent on global names that are specific to a concrete program.

*Good programming practice recommends using local names rather than global names. Here are some tips:*

    - Write self-contained functions that rely on local names rather than global ones.

    - Try to use unique objects names, no matter what scope you’re in.

    - Avoid global name modifications throughout your programs.

    - Avoid cross-module name modifications.

    - Use global names as constants that don’t change during your program’s execution.

The *built-in scope* is a special Python scope that’s implemented as a standard library module named builtins in Python 3.x. All of Python’s built-in objects live in this module. They’re automatically loaded to the built-in scope when you run the Python interpreter.

[Don’t be CONFUSED by BIG O notation anymore!](https://www.youtube.com/watch?v=5Uqawfl0VHQ)


...............................................................................

__Attributions for the following Reference materials and their authors__

[Python Scope & the LEGB Rule: Resolving Names in Your Code- by Leodanis Pozo Ramos](https://realpython.com/python-scope-legb-rule/)


[>> NEXT (Read: Class 08)](https://wondwosentsige.github.io/code-401-reading-note/class-08)
