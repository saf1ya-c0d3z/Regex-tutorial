# My Email Regex Expression
 
In this assignment I will be "decoding" a specific regex expression that can be used in JavaScript. This specidic regex expression may be used to locate, manage or match text using a string text to create patterns.

## Summary

A regular expression (regex for short) is a sequence of characters that defines a search pattern.
A meta character indicates a generalized pattern rather than a literal character.
A literal character is exactly what is sounds like. So a literal character in a regex may mean that 6 actually is 6 in the string.


The regex I will be describing is for validating an Email:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## regex explanation overView

/ - delimiter used to enclose regular expressions in many programming languages (used in JavaScript)

@  - this is a literal character where the "@" in the email is

\ - used to escape characters that have a special meaning  (without the backslash escape the literal character (.) that follows would match any character and not be defined specifically as a dot, which is neccasary in this email)

. - literal character- meant to match the literal dot (.) in the regex expression ( ex: in this expression this is the dot before "com" in ".com" or "org" in ".org")

(   - this is the beginning of a capturing group which groups tokens together for extracting a substring or using a back reference

[ - this is the beginning of a character set

0-9 - is a  "range: this can be a single charcter between 0 and 9

]  - this is the end of a charcter set

) - this is the end of the capturing group

(  - this is the beginning of a capturing group which groups tokens together for extracting a substring or using a back reference

[ - this is the beginning of a character set

\d - matches any digit character (0-9)

a-z -is a "range" this can be a single character between a and z

]  - this is the end of a charcter set

) - this is the end of the capturing group

$ - this is the anchor which matches the end of the string
 
 / - this signifies the end of the regex pattern in JS


a-z -is a "range" this can be a single character between a and z
## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors

^  -signifies the beginning of the string

$ - the anchor which matches the end of the string

### Quantifiers

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
