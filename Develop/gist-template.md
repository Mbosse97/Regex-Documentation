# Email Regular Expression Documentation

The following documentation will go through the Regular expression responsible for the search pattern associated with emails and their verification. 

The expression for this can be seen here below:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Each section will break down the components of this expression and determine their purpose and effect.

## Summary

The Regular Expression ("/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/") is used to determine the validity of email entries, with each section 

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

Anchors are Regex tokens which dont match any characters of the string, however will assert a location of the string in the matching process 

The caret or "^" Marks the beginning of  string

The dollar or "$" Marks the end of the string

---

### Quantifiers

Quantifiers will match one or more of the preceeding characters or group. 

Within this expression the plus or "+" symbol will repeat the previous item once or more times, up to the point where the preceeding item is only matched once. 

---

### OR Operator

the OR Operator "|" will create an OR condition within the expression. however there are no OR Operators within the expression chosen. 

---

### Character Classes

Character classes are chosen to instruct the engine to match only within characters defined in the class or set provided.

These classes include:
- [a-z0-9_.-] : Which matches any lowercase letter, digit, underscore, dot or hyphen.
- \d : Which matches any digit.
- [a-z.] : Which matches any lowercase letter or dot.

---

### Flags

Flags are used to alter the expression's ouptut and what is allowed as input into the expression, e.g. "i" ehich makes the search case insensitive or g will look for all matches, instead of the default one match. 

However, there are no flags in this expression. 

---

### Grouping and Capturing

Capturing groups is done by used the () parenthesis with the expression conditions within them to determine the captured group. 

Within this expression, the Groups and the data being captured are as follows. 

- ([a-z0-9_.-]+) : Captures one or more occurrences of any lowercase letter, digit, underscore, dot or hyphen, before the "@" symbol.
- ([\da-z.-]+) : Captures one or more occurrences of any digit, lowercase letter, dot or hyphen, between the "@" symbol and the first dot in the domain name.
- ([a-z.]{2,6}) : Captures a sequence of lowercase letters or dots, between the first and second dots in the domain name. The sequence must be between 2 and 6 characters long.

---

### Bracket Expressions

- [] brackets indiciate a set of brackets to match
- {} are used to specifiy the exact amount of things to match
- () respresent remembered matches 

---

### Greedy and Lazy Match

The Expression also uses Greedy Quantifiers with the "+" symbol as it specifies one or more occurances of the preceeding group, with the quantifier being greedy by default. 

---

### Boundaries

With the use of he word boundary "\b" it can match a word within a specified position based on its use. 

However, there are no word boundaries used in this expression. 

---

### Back-references

Back references as used to recall earlier capturing groups within the expression with a "/" followed by a digit e.g. "/1"

However, there are no Back-references within this expression

---

### Look-ahead and Look-behind

These are assertions within the expression which will simply return whether the expression is a match or not a match. 

However, there are no Lookaround calls within this expression. 

---

## Author

Author: Michael Bosse - Coding bootcamp Student 

Github: https://github.com/Mbosse97
