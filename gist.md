# Another Regex Tutorial

As a part of the coding community, I believe it is important to share relevant and useful information among ourselves, therefor I decided to write a tutorial to explain a RegEx. 

## Summary

Let's take the following code as an example: 

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

What we have here is a regular expression to match email addresses. Below we will go over the syntax of how this expression is written and how it will help your algorithm find email addresses.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes & Bracket Expressions](#character-classes--bracket-expressions)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)


## Regex Components

### Anchors
The '^' symbol and '$' mark the beginning and the end of the string that wil contain an email in this case. These are unique and match positions within strings, not characters.

### Quantifiers
Quantifiers in this expression include the following characters: + and {}. Plus sign matches one (or more) of the preceding token. In this case it will match the beginning of an email address with as many characters as possible given the combination that is searched. 

The curly brackets at the end of the expression indicates how many characters it will permit within the previous token. In this case the .com, .org, .edu ending of an email will allow for it to have 2 to 6 characters long. 

### Character Classes & Bracket Expressions
In this expression the character classes are contained within the bracket expressions '[]'. These search for a range or specific set of characters containing any of the listed i.e. letters a-z, numbers 0-9, \d (for digit searches).

### Grouping and Capturing
Grouping characters between parenthesis allows this expression to combine the beginning, and final part of the email address. In this example character classes are different within each bracket expression due to the different possible combination of email addresses. 

### Greedy and Lazy Match
The quantifiers in the termination of the email address '{}' are the only greedy and/or lazy match used. These make the termination of the email address strictly 2-6 characters. 

## Author

Tutorial Developed:
Francisco Rivera
-Fullstack Developer
Github: github.com/frivera14