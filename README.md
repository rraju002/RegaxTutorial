# Regex Tutorial Starter Code

## Regex Tutorial

As a Full-Stack Web Developer I found it important to explain the specifics of regex to ensure we understand what the search patterns are within the regex!

## Summary

Regex stands for "regular expression," a sequence of characters which define a specified search pattern. Most patterns are used via string-search algorithims such as the "find" function.  

Moving forward we will be looking at the email validation regex or, </br> `\b[a-z0-9#$_-]+@[a-z0-9]+\.[a-z]{2,3}\b/gi`</br>

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
Analyzing... </br> `\b[a-z0-9#$_-]+@[a-z0-9]+\.[a-z]{2,3}\b/gi`</br> 
- First lets start with defining some key terms... 
 - The Alpha and Omega can in short be considered the beginning and end which ends in '\b' also known as "word boundaries." Word boundaries explain expressions need to be partnered as a stand-alone string, for example closed parentesis, without seperating spaces their validation is likely to fail due to it's inability to match with another component.

- Considering the 1st group... `[a-zA-Z0-9#$_-]+` 
- Correlates w/ any upper or lower case letter along with any number and characters `#$_-`. The `-` used between the "a" and "z" fulfill the requirement of any letter variable between the two. With that said,`0-9` have the same meaning in regards to numerical values. The quantifier, (`+`) symbolizes any of the characters before may occur more than once ie `Rhowen_raju13`. 

- The `@` is required for emails.
- `[a-z0-9]+` matches with any upper or lowercase letter and does the same with any number, therefore if one's username was `rojo29` the username would be accepted!
-  `\.`, is the dot before the extension(`com`,`gov`,`ca`, etc.,).
- `[a-z]{2,3}` holds the extension. `[a-z]` signfies any letter between A-Z will be accepted. The {2,3}`is a fixed quantifier, indicating the min. and max. length of the extension. 
- Examples: `rhowen_13``@``rojo29``.``com` or simple `rhowen_13@rojo29.com`!

### Anchors

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
