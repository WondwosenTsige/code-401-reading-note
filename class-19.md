# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 19: Automation

### Regular Expressions in Python

Regular Expressions, often shortened as regex, are a sequence of characters used to check whether a pattern exists in a given text (string) or not. If you've ever used search engines, search and replace tools of word processors and text editors - you've already seen regular expressions in use. They are used at the server side to validate the format of email addresses or passwords during registration, used for parsing text data files to find, replace, or delete certain string, etc. They help in manipulating textual data, which is often a prerequisite for data science projects involving text mining.

In Python, regular expressions are supported by the re module. That means that if you want to start using them in your Python scripts, you have to import this module with the help of import

    import re

#### Basic Patterns: Ordinary Characters

You can easily tackle many basic patterns in Python using ordinary characters. Ordinary characters are the simplest regular expressions. They match themselves exactly and do not have a special meaning in their regular expression syntax.

        Examples are 'A', 'a', 'X', '5'.

#### Wild Card Characters: Special Characters

Special characters are characters that do not match themselves as seen but have a special meaning when used in a regular expression. For simple understanding, they can be thought of as reserved metacharacters that denote something else and not what they look like.

. - A period. Matches any single character except the newline character.

^ - A caret. Matches the start of the string.

$ - Matches the end of string

[abc] - Matches a or b or c.
[a-zA-Z0-9] - Matches any letter from (a to z) or (A to Z) or (0 to 9).

*TIP: Characters that are not within a range can be matched by complementing the set. If the first character of the set is ^, all the characters that are not in the set will be matched.*

\ - Backslash.
Perhaps, the most diverse metacharacter!!

If the character following the backslash is a recognized escape character, then the special meaning of the term is taken

Else if the character following the \ is not a recognized escape character, then the \ is treated like any other character and passed through.

\ can be used in front of all the metacharacters to remove their special meaning.









...............................................................................

__Attributions for the following Reference materials and their authors__

[Python Regular Expression Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)

[]()

[>> NEXT (Read: Class 20)](https://wondwosentsige.github.io/code-401-reading-note/class-20)