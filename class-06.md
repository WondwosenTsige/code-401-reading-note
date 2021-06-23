# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## How to use Random module

The Random module provides access to functions that support many operations. Perhaps the most important thing is that it allows you to generate random numbers.

The Random module contains some very useful functions like:-

    Randint - accepts two paramrters, a lowest and highest number to generate a random integer

        import random
        print random.randint(3, 10) -----> probable outputs  4,5,6,7,8,9,10 or some other random order

    Random - Use this one if we want a large number.

        import random
        random.random()*150

    Choice - Generate random value from the sequence sequence. It is often used for choosing random element from a list

        random.choice(["apple", "orange", "banana" ])

    Shuffle - shuffles the elements in list in a random order

        from random import shuffle
        y = [[j] for j in range(5)]
        shuffle(y)                  ---------> probable output [[4], [1], [0], [3], [2]] or the oder will vary

    Randrange - Generate a randomly selected element from a range

## What is Risk Analysis in Software Testing

In Software Testing, risk analysis is the process of identifying the risks in applications or software that you built and prioritizing them to test.

### Why use Risk Analysis

Identifying the potential problem areas helps the developers and managers to mitigate the risks.

When a test plan has been created, risks involved in testing the product are to be taken into consideration along with the possibility of the damage they may cause to thr software along with solutions.

### Risk identification

There are different sets of risks included in the risk identification process.

    Business Risks: This is the risk that may come from our company or our customer, not from our project.

    Testing Risks: we should be well organized with the platform we are working on, along with the software testing tools being used.

    Premature Release Risk: a fair amount of knowledge to analyze the risk associated with releasing unsatisfactory or untested software is required

    Software Risks: we should be well versed with the risks associated with the software development process.

### Risk Assesment

There are three perspectives of Risk Assessment

    Effect - To assess risk by Effect. In case if a condition is identified, event or action and try to determine its impact.

    Cause - To assess risk by Cause is opposite of by Effect. Initialize scanning the problem and reach to the point that could be the most probable reason behind that.

    Likelihood – To assessing risk by Likelihood is saying that there is a probability that a requirement won’t be satisfied.

### How to perform Risk Analysis?

The three steps of performing Risk analysis are:

    Searching the risk

    Analyzing the impact of each individual risk

    Measures for the risk identified


[Bog O Notation](https://www.youtube.com/watch?v=v4cd1O4zkGw)





...............................................................................

__Attributions for the following Reference materials and their authors__

[PythonForBeginners](https://www.pythonforbeginners.com/random/how-to-use-the-random-module-in-python)
[What is Risk aAnalysis in software testing and how to perform it? - by Anamika Kalwan](https://www.edureka.co/blog/risk-analysis-in-software-testing/)


[>> NEXT (Read: Class 07)](https://wondwosentsige.github.io/code-401-reading-note/class-07)
