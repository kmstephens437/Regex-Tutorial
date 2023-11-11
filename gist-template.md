# Regex Tutorial

This Tutorial will be covering what a Regex (Regular Expression) is, an example of a Regex, and how to use it. A regular expression is a set of special characters that are representative of either literal or meta characters within a particular writing/coding environment. It is used to match specific requirements to exisiting alpha/numeric text/code for various purposes. For example, to pull all phone numbers that may be formatted differently from a spreadsheet or to verify that someone entered their birth date in the format you'd like on a form. There are endless reasons you may want to use this matching functionality. We'll take a look at one below. 

## Summary

In this tutorial, we'll take a look at the following Regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The criteria set forth in this Regex can be used to match data with the proper formatting of an email address. We will break down each component below with a summary of what they are called and their purpose. 

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

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Anchors indicate the beginning and the ending of the expression. In our code above it is the ^ and the $. Our code is defining what to look for in the beginning and end of our string. 

### Quantifiers

Quantifiers match a number of instances of a character, group, or character class in a string. The quantifier in our code + indicates that there has to be at least one of all of the following [\da-z\.-].

### Grouping Constructs

Sections of a Regex can be grouped together as in with our code we have three groups or sections that are clearly marked with parenthesis. When used in Regex, the conditions of each group must be satisfied before continuing to try to match the next group. 

### Bracket Expressions

Brackets in Regex enclose a set of characters to match. Any one individual character will reult in a match.

### Character Classes

Character class will define the type of character to match. For our example \d will be matching with anything that is not a number or special character after our @ symbol.  

### The OR Operator

In Regex the OR operator is represented by the pipe symbol |. It is quite literally doing what it's name indicates.....describing acceptable "OR" conditions to be matched to. For example 4|Four. We don not have any examples of the OR operator in our code for this Regex. 

### Flags

There are 6 possible flags within a regex.

i - will make your search disregard case. 
g - will make your search look for all occurrences.
s - makes the wild character . match new lines as well.
m - will make the ^ and $ match the start and end to every line instead of just the whole string.
y - will start search from the index in Last Index property. 
u - makes search match 32-bit charactrers. 

### Character Escapes

Character escape represents a character that potentially shouldn't be described in it's literal definition.

## Author

Kevin Stephens
https://github.com/kmstephens437


