# Regex_Tutorial

Introductory paragraph (replace this with your text)

## Summary

I will be describing a regular expression that reprensents an email, which is of the form `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`


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

The anchor characters "^" and "$" are the second and second to last characters in the regular expression respectively. The "^" indicates at a matching string will begin with the characters that follow it while "$" indicates that a matching string will begin with the characters that precede it. In our example case, "^" is followed by a subexpression that indicates that a string of any length greater than 1 containing lowercase alphanumeric character and the characters "_", ".", and "-", will start the string, while "$" is preceded by a subexpression that indicates that a number, any number of lowercase alphabetic characters, and any number of the character "." of length 2 to 6 will end the string.

### Quantifiers

A qauntifier sets a value to the number of characters an expression or subexpression can have. Our example contains two such quantifiers, "+", which indicates a length of 1 or greater, and "{2,6}", which indicates a length of 2 to 6. "{x,y}" can be used to indicate a character count that is inclusively within the range x to y.

### Grouping Constructs

Group constructs are indicated with paratheses and are used to create subexpressions that act independently of the rest of the expression. Our example contains three group constructs; from left to right, the first one represents the email username, the second represents the domain name or service provider's name, and the last reperesnts the extension.

### Bracket Expressions

Bracket expressions are indicated with square brackets and are used to represent an occurances of the characters within them. Our example contains several bracket expressions, with one being "[a-z0-9_\.-]" which represents a single lowerlowercase alphanumeric character or one of the characters "_", ".", and "-". Bracket epxressions may have their length modified using quantifiers.

### Character Classes

Character classes are used to define a set of characters. There are several character classes but only one, "\d", is used in our example. "\d" indicates a any arabic numeral between 0 and 9.

### The OR Operator

The OR operator is used to indicate and or-statement within a regualr expression. Our example does not contain the OR operator.

### Flags

Flages are used to indicate additional limits on a regualr expression, and are placed after the closing "/". Our example does not contain any flags.

### Character Escapes

Character escapes are used to show that a character should be interpreted as a meta character in a regular expression instead of as some component of regualr expression syntax. Our example includes one unqiue character escapes, "\.", which is used to indicate the "." literal character instead of the universal match meta character "."

## Author

About: I am enrolled at the UMN's coding bootcamp
Github Profile Link: https://github.com/fortu038
