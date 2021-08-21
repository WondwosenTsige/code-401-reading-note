# [Table of Contents](https://wondwosentsige.github.io/code-401-reading-notes/Home)

## Read 19: Automation

[Super quick Python automation ideas](https://www.youtube.com/watch?v=qbW6FRbaSl0&t=69s)

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

There is a predefined set of special sequences that begin with '\' and are also very helpful when performing search and match. Let's look at some of them up close...

\w - Lowercase 'w'. Matches any single letter, digit, or underscore.

\W - Uppercase 'W'. Matches any character not part of \w (lowercase w).

\s - Lowercase 's'. Matches a single whitespace character like: space, newline, tab, return.

\S - Uppercase 'S'. Matches any character not part of \s (lowercase s).

\d - Lowercase d. Matches decimal digit 0-9.

\D - Uppercase d. Matches any character that is not a decimal digit.

\t - Lowercase t. Matches tab.

\n - Lowercase n. Matches newline.

\r - Lowercase r. Matches return.

\A - Uppercase a. Matches only at the start of the string. Works across multiple lines as well.

\Z - Uppercase z. Matches only at the end of the string.

*TIP: ^ and \A are effectively the same, and so are $ and \Z. Except when dealing with MULTILINE mode. Learn more about it in the flags section.*

\b - Lowercase b. Matches only the beginning or end of the word.

Refer to the examples in the following link

[Python Regular Expression Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)


...............................................................................

__Attributions for the following Reference materials and their authors__

[Python Regular Expression Tutorial](https://www.datacamp.com/community/tutorials/python-regular-expression-tutorial)


[]()

[>> NEXT (Read: Class 26)](https://wondwosentsige.github.io/code-401-reading-note/class-26)