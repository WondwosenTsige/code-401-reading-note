# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 28: Django CRUD and Forms

An HTML Form is a group of one or more fields/widgets on a web page, which can be used to collect information from users for submission to a server. Forms are a flexible mechanism for collecting user input because there are suitable widgets for entering many different types of data, including text boxes, checkboxes, radio buttons, date pickers and so on. Forms are also a relatively secure way of sharing data with the server, as they allow us to send data in POST requests with cross-site request forgery protection.

The main things that Django's form handling does are:

    Display the default form the first time it is requested by the user.

    Receive data from a submit request and bind it to the form.

    Clean and validate the data.

    If any data is invalid, re-display the form, this time with any user populated values and error messages for the problem fields.

    If all data is valid, perform required actions (e.g. save the data, send an email, return the result of a search, upload a file, etc.)

    Once all actions are complete, redirect the user to another page.

Django provides a number of tools and approaches to help you with the tasks detailed above. The most fundamental is the Form class, which simplifies both generation of form HTML and data cleaning/validation











...............................................................................

__Attributions for the following Reference materials and their authors__

[Django Tutorial Part 9: Working with forms](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Django/Forms)


[>> NEXT (Read: Class 29)](https://wondwosentsige.github.io/code-401-reading-note/class-29)