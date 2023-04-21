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

+ - matches one or more occurences of the previous character or group fo characters

{2,6} - this is a quantifier which specifices the miniimum and maximum number of occurences of the preceding pattern which should be matched. Since the preceding characters are "\.([a-z\."] this means the pattern should match a dot followed by 2-6 lowercase alphabetical characters or dots. (this is likely where we would find .com or .org, .edu or .pb.se). Since this is followed by a '$' this signifies this pattern will come at the end of each string.

### OR Operator

(note: there is no or opperator in the specific regex shown in this gist-template)

 OR operator '|' allows you to have a match of one pattern or a different pattern (| = or)

### Character Classes

(Matches...)

[a-z0-9_\.-] -  any lowercase number, digit, underscore, dot or hyphen

[\da-z\.-] - any character that is a digit, lowercase letter dot or hyphen

[a-z\.] - any character that is a lowercase letter or a period (.)

### Flags

(note: there are so flags used in the specific regex shown in this gist-template)

'g','i','m','s','u','y' - characters that modify and change the behavior of a regex by appending to the end, each character has a different effect on the regex

### Grouping and Capturing

'([a-z0-9_\.-]+)', '([\da-z\.-]+)', '([a-z\.]{2,6})'

()- Allows you to capture and use parts of a matched string (captures the substring for future use)

### Bracket Expressions

[]- used to match any character that belongs to a specified set

### Greedy and Lazy Match

Controls how many characters are matched

Greedy matching- matches as many characters as possible
Lazy matching - opposite of Greedy matching, - matches the minimum characters required for pattern to match (lazy match by adding '?' after the quantifier)

### Boundaries

Used to match patterns that are at the beginning or end of the line

^  -signifies the beginning of the string

$ - the anchor which matches the end of the string

### Back-references

(note: there are no back-references used in the specific regex shown in this gist-template)

Refers to a previous match in the pattern and use it later
ex:\b, \1, \s+, (\w+)

### Look-ahead and Look-behind

There are positive and negative looks ahead and positive and negative looks behind

Look-ahead/Look-behind allows you to match patterns based on what is before and after the pattern
it does this without including text in the match

key: "pattern" represents a variable which is the pattern in the specific regex

ex: (?="pattern"), (?!"pattern"), (?<="pattern"),  (?<!"pattern"). 

## Author

Zoe-Sophia Shrader is a 21 year old who has began taking UC Berkley's Coding Bootcamp in 2022. She is close to completing this course and is currently working on her 18th module with approximately one month left in her bootcamp until she can recieve her certificate. After this she hopes to be able to hone her skills and continue her learning so that she may have the oppurtunity to work in the tech field.

Her gitHub profile is: https://github.com/
