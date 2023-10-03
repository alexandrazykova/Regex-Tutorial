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
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

"^" and "$" anchors are used to specify the start and end of a line or string.

### Quantifiers

These are used to specify how many times a character or group should occur. Examples include *, +, ?, and {}

In the email validation expression, we are using the following:

Quantifier "+" to match 1 or more of the precending token.

{2,6} quantifier to match between 2 and 6 of the precending token.

### Character Classes

These allow to specify a set of characters that can match at a certain position. In out case, we are using \d which matches any digit character 0-9.

### Grouping and Capturing

Parentheses () are used to create capture groups, which allow you to extract portions of a matched text.

1) First capturing group ([a-z0-9_\.-]+):

Range a-z: matches a character in the range "a" to "z", case sensitive.

Range 0-9: matches a character in the range "0" to "9".

Character _ : matches a "_" characters.

\. character: matches any character(digits, letters,special characters, whitespace, etc.) except for a newline character \n.

Character - : matches a "-" character.
  
Quantifier "+" to match 1 or more of the precending token placed outside of [].

@ character: matches a "@" character.

2) Second capturing group ([\da-z\.-]+):

\d : matches any digit character 0-9.

Range a-z: matches a character in the range "a" to "z", case sensitive.

\. character: matches any character(digits, letters,special characters, whitespace, etc.) except for a newline character \n.

Character "-" : matches a "-" character.
  
Quantifier + to match 1 or more of the precending token placed outside of [].

\. character to match a literal dot, has to be escaped by using a slash in order to match a period.

3) Third capturing goup ([a-z\.]{2,6}):

Range a-z: matches a character in the range "a" to "z", case sensitive.

\. character: matches any character(digits, letters,special characters, whitespace, etc.) except for a newline character \n.

{2,6} quantifier to match between 2 and 6 of the precending token.

### Bracket Expressions

Characters defined inside a set of square brackets [] are the once that we want to match. It is also known as a positive character group, because they outline the characters we want to include. Our email regex includes three sets.

One ([a-z0-9_\.-]+),
Two ([\da-z\.-]+),
Three ([a-z\.]{2,6}).

### Greedy and Lazy Match

Regular expressions have 2 ways of searching for a match:

Greedy - to match the longest possible string.
Lazy - to match the smallest possible string.

In our email matching regex, first and second capturing groups are using greedy + quantifier to match as many characters as possible while still allowing the rest of the pattern to match.

Also, {} quantifier is used in the third capturing group to specify matching range, which is from 2 to 6 characters.

## Author

Get in touch for more tech talk, to view my work and and to collaborate https://github.com/alexandrazykova
