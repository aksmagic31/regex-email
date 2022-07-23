## Regex Tutorial - Matching An Email

## Summary
Below is the regex expression used for validating an email address.
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
Regex, or Regular Expression,  is a sequence of characters that defines a specific search pattern. This tutorial is designed to help fellow coders understand the specific instance of Regex usage to match an e-mail.  When regular expressions are included in code or search algorithms, they can be utilized to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. At the same time, they can also be used to validate input data.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)


## Regex Components

### Anchors
Anchors matches us the beginning, end or between characters. Anchors that are used in this regex expression for matching an email are ^ , which indicates the beginning of the string and $, which is to indicate the ending of the string.

in the code of ^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$ 
### Quantifiers
Quantifiers tells us how many times a character, group, or character class must be present in the input for a match to be found. In the example code, the + represents one or more times and the {2,6} represent two to six times. i.e {2,6}) in the code. 

### Grouping Constructs
Grouping Contructs can let you grab subset of information from a token or text. In fact, There are three grouping construtions in the regex, each being defined with the ( ): For instance, ([a-z0-9_\.-]+) defines the user's email name.

### Bracket Expressions

Bracked expressions indicates a set of characters to match. it is indicated by the brackets, or []. In the email validation, there is a bracket expression [a-z0-9_\.-], which is matching any letter a-z and numbers 0-9 and is case senstive. 

### Character Classes
The character class are also called "character set", and they are used to tell the regex engine to match only one out of several characters. For example,  in this expression the character class is \d, like, \da-z\ which is enclosed within the square bracket and means one out of several characters. 

### The OR Operator
The OR Operator in Regex is defined by "|" or "\| ” and they are also called the Alternation Operator. There is no Or Operator in the expression given but if we need to create one we can write something like `1|2|3' which means 1 or 2 or 3.

### Flags
There are different flag varibles, namely: g , i , m , u , s , y. Those are option flags that each have a meaning and will affect the search result. g flag means look for all matches, so without it only first result is returned. i flag indicates search is not case sensitive. u flag uses full unicode support and m flag means multiline mode. For example, regexp = /pattern/gmi; has g m i flag so the search result will return all results which are case sensitive and have multiline mode. 

### Character Escapes
The \ symbol,known as the escape code, preceeds some literal character. In the expression, \da-z it means single digit of the character a-z. Ther can be also usage of Escape Characters to represent common character classes, such as \w for a word character or \s for a space.

## Author
Wenyu Zhang
Github Username: aksmagic31
Github Link: https://github.com/aksmagic31
