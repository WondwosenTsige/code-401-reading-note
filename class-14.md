# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Data Visualization - Matplotlib

matplotlib is probably the single most used Python package for 2D-graphics. It provides both a very quick way to visualize data from Python and publication-quality figures in many formats

IPython is an enhanced interactive Python shell that has lots of interesting features including named inputs and outputs, access to shell commands, improved debugging and much more.

pyplot provides a convenient interface to the matplotlib object-oriented plotting library. It is modeled closely after Matlab(TM). Therefore, the majority of plotting commands in pyplot have Matlab(TM) analogs with similar arguments.

[Pyplot tutorial](https://matplotlib.org/2.0.2/users/pyplot_tutorial.html)

Matplotlib comes with a set of default settings that allow customizing all kinds of properties. You can control the defaults of almost every property in matplotlib: figure size and dpi, line width, color and style, axes, axis and grid properties, text and font properties and so on

While matplotlib defaults are rather good in most cases, you may want to modify some properties for specific cases.

we can instantiated all the figure settings that influence the appearance of the plot icluding the figure size, color, line width and style like:

    plt.figure(figsize=(10,6), dpi=80)
    plt.plot(X, C, color="blue", linewidth=2.5, linestyle="-")
    plt.plot(X, S, color="red",  linewidth=2.5, linestyle="-")






















...............................................................................

__Attributions for the following Reference materials and their authors__

[matplotlib tutorial - Nicolas P. Rougier](https://github.com/rougier/matplotlib-tutorial)



[>> NEXT (Read: Class 15)](https://wondwosentsige.github.io/code-401-reading-note/class-15)