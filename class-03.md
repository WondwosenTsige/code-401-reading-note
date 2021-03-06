# Read Class 03

## FileIO & Exceptions

### What is a file?

a file is a contiguous set of bytes used to store data. This data is then organized in a specific format and can be anything as simple as a text file or as complicated as a program executable and then translated into binary 1 and 0 for easier processing by the computer.

Most of the modern file systems are composed of three main parts:

Header: metadata about the contents of the file (file name, size, type, and so on)
Data: contents of the file as written by the creator or editor
End of file (EOF): special character that indicates the end of the file

What data represents depends on the format specification used, which is represented by an extension. For example, a file that has an extension of .txt most likely conforms to the text format specification.

### File Paths

The file path is a string that represents the location of a file. It’s broken up into three major parts:

Folder Path: the file folder location on the file system where subsequent folders are separated by a forward slash / (Unix) or backslash \ (Windows)
File Name: the actual name of the file
Extension: the end of the file path pre-pended with a period (.) used to indicate the file type. Example:- Resume.docs

To access up one directoy up without using the full path, we can use the special character double-dot(..).

    for example, to accees the contacts.csv file in the directory up, we can use ../contacts.csv is equivalent instead of directory/contacts.csv.
    and if you want to access two directoreies above it will be ../../contacts.csv

### Line Endings

One problem often encountered when working with file data is the representation of a new line or line ending.

Both the International Organization for Standardization (ISO) and the American Standards Association (ASA) standardized the representation of a new line or line ending. 

ASA standard states that line endings should use the sequence of the Carriage Return (CR or \r) and the Line Feed (LF or \n) characters (CR+LF or \r\n). The ISO standard however allowed for either the CR+LF characters or just the LF character.

Those different standards can cause problems when we are trying to process on an operating system that is different from the file's source.

In the example below, we will see how Windows, which uses CR+LF cahracter to indicate a new line and how the same file is interperated by Unix and the newer Mac version which uses the LF cahracter.

    The file contacts_list. created on a Windows system:

        James Gordon\r\n
        Jack Bower\r\n
        Wondwosen Tsige\r\n
        Ben Hill\r\n

The same output will be interprated by Unix device as

        James Gordon\r
        \n
        Jack Bower\r
        \n
        Wondwosen Tsige\r
        \n
        Ben Hill\r
        \n

### Character Encodings

Another common problem that you may face is the encoding of the byte data. An encoding is a translation from byte data to human readable characters by assigning a numerical value to represent a character.by assigning a numerical value to represent a character.

The most common encodings are the ASCII(American Standard Code for Information Interchange) and Unicode foramats which can store 128 and upto 1,114,114 characters respectively.
ASCII is the subset of Unicode(UTF-8), so that they share the first 128 numerical characters.Because of that, if we try to parse it using the ASCII encoding, if there is a character that is outside of those 128 values, then an error will be thrown.

### Opening and Closing a File in Python

Opening a file in Python is invoking the built-in function *open()*. Open() has a single required argument that is the path to the file. open() has a single return, the file object:

    file = open('contacts_list.csv')

After opening a file,  it’s our responsibility to close the file. In most cases, upon termination of an application or script, a file will be closed eventually. However, there is no guarantee when exactly that will happen. The two ways to close a file are

    1. Use the *try-finally* block

        reader = open('contacts_list.csv')
        try:
            # Further file processing goes here
        finally:
            reader.close()

    2. Use the *with* statement which is the highly recommended way, and it automatically takes care of closing the file once it leaves the with block, even in cases of error. This option it allow us for cleaner code and makes handling any unexpected errors easier for us.

        with open('contacts_list.csv') as reader:

Other most commonly used options for modes are:

    Character       Meaning
    'r'             Open for reading (default)
    w'              Open for writing, truncating (overwriting) the file first
    'rb' or 'wb'    Open in binary mode (read/write using byte data)

There are three different categories of file objects:

    Text files
    Buffered binary files
    Raw binary files

## Exceptions in Python

A Python program terminates as soon as it encounters an error. In Python, an error can be a syntax error or an exception

In Python, _syntax errors_ occur when the parser detects an incorrect statement and an arrow will indicate us where the parser ran into the syntax error

*Exeption error* occurs whenever syntactically correct Python code results in an error with details of what type of exception error was encountered.

we can raise an exception using *raise* if you want to throw an error when a certain condition occurs, like

    x = 10
    if x > 5:
        raise Exception('x should not exceed 5. The value of x was: {}'.format(x))

Running the above code, will halt the program and display the following exception on the screen with clues aboout what went wrong

    Traceback (most recent call last):
        File "<input>", line 4, in <module>
    Exception: x should not exceed 5. The value of x was: 10

*assert* enable us to verify if a certain condition is True and throw an exception if it is not like the following example

    import sys
    assert ('linux' in sys.platform), "This code runs on Linux only."

If we run the above code on a Linux machine, the assertion passes. If we run this code on a Windows machine, the outcome of the assertion would be False and the result would be the following:

    Traceback (most recent call last):
        File "<input>", line 2, in <module>
    AssertionError: This code runs on Linux only.

The *try and except* block in Python is used to catch and handle exceptions. Python executes code following the try statement as a “normal” part of the program. The code that follows the except statement is the program’s response to any exceptions in the preceding try clause.

_The good thing in the try and expect case is that the program did not crash. It would be nice to generate an informative message if some type of exception occurred whenever we ran our code_, like "Linux function was not executed", which the following example will print if we try to call it on a different operating system other than Linux.

    try:
        linux_interaction()
    except:
        print('Linux function was not executed

*else* let us to run sections that should run only when no exceptions are encountered in the try clause. like:

        try:
            linux_interaction()
        except AssertionError as error:
            print(error)
        else:
            print('Executing the else clause.

*finally* will execute everything in the finally clause, wether we encounter an exception somewhere in the try or else clauses. like:

    try:
        linux_interaction()
    except AssertionError as error:
        print(error)
    else:
        try:
            with open('file.log') as file:
                read_data = file.read()
        except FileNotFoundError as fnf_error:
            print(fnf_error)
    finally:
        print('Cleaning up, irrespective of any exceptions.')

The output of the above code is:

    Function can only run on Linux systems.
    Cleaning up, irrespective of any exceptions.







...............................................................................

__Attributions for the following Reference materials and their authors__

[Reading and writing files in Python(Guide) by James Mertz](https://realpython.com/read-write-files-python/)

[Python Exceptions by Said van de klundert](https://realpython.com/python-exceptions/)

[>> NEXT (Read: Class 04)](https://wondwosentsige.github.io/code-401-reading-note/class-04)