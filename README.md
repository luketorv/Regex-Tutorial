# Regex Tutorial

Regex is a sequence of characters that defines a specific search pattern. They can be used to validate input. In this tutorial we'll be using regex to validate an email address.

## Summary

Here is the code we'll be analyzing today:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

The anchors in this expression are `^` and `$`. They are used to start and end the expression.

### Quantifiers

The quantifiers used in this expression are `+` and `{2,6}`.

The + is used to show there is another sequence to be matched, and {2,6} shows input should be minimum 2 charactors & maximum 6 characters.

### Character Classes

In our regex code, `\d` is used to match any digits 0-9.

### Grouping and Capturing

The groups in this expression are: 
`a-z0-9_\.-` for the username. 
`\da-z\.-` for the email service.
`a-z\.` for the domain name.

### Bracket Expressions

Bracket expressions are characters inside of []

The bracket expressions in this expression are:
[a-z0-9_\.-]
[\da-z\.-]
[a-z\.]

### Greedy and Lazy Match

Greedy and Lazy matches refer the longest and shortest possible string that could be made with regex code.

In our expression, `+` is used for a greedy search

To switch to a lazy search, add `>` 

## Author

Luke Torvinen is an audio engineer and full stack web developer.

https://github.com/luketorv