# Email Validation. Regex Tutorial

Regular expression (regex) is a great and flexible way for validating an input. This tutorial will guide you to get a better understanding of an email regular expression, that can be customized for any format you decide to use. 

How is it useful? It will allow a quick and easy validation of entered emalis to be legitimate, with proper and consistent formatting, and avoid typos.

## Summary 

Regular expression is a set of characters that is widely used to search for, match, validate, clean, and manipulate input. Let's break down to take a closer look at matching an email regex, and components needed to build a pattern to match character combinations in strings.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ expression contains beginning of the string, local part of the email address, symbol '@' which separates local and domain parts, literal period (.), top-level domain, and, finally, end of the string. 


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
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
Anchors: ^ and $ are used to specify the start and end of a line or string.

### Quantifiers
Quantifiers: These are used to specify how many times a character or group should occur. Examples include *, +, ?, and {}

### Character Classes
character Classes: These allow you to specify a set of characters that can match at a certain position. For example, [aeiou] matches any vowel.

### Flags

### Grouping and Capturing

Capture Groups: Parentheses () are used to create capture groups, which allow you to extract portions of a matched text.

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Get in touch for more tech talk, to view my work and and to collaborate https://github.com/alexandrazykova
