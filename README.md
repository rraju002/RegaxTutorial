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
- `\b` is an anchor, serving the purpose of defining a "word boundary," provoking a "whole word" search. 
- Example:
if the Regex was `\b867530\b`, then only `867530` would match up but not `8675309`. 
- Other anchor examples:
`^` 
`$`

- ^RRRRR will match any string that starts with ^RRRRR

- RRRRR$ will match any string that ends with RRRRR$

- Anchors are a type of meta-character not matching any characters, rather matching specific positions.`^` matches the starting position right before the 1st character of the search string, in comparisson `$` matches the end of the last character, and `\b` defining the entire boundary of the search string.
### Quantifiers
- Quantifiers repeat the previous item 1 or more times. There's a large list of quanitifiers however `+` is part of that group, which states that the previous item(the collection of characters) can be repeated multiple times. Also known as a "greedy quantifier" because an item can be matched to it multiple times.

- {2,3}` is a fixed quantifier, specifically stating the search must be between 2 and 3 characters.

- There are also simpler quantifiers, for example `{3,}`, stating the preceeding item repeats at least 2 times. Also considered to be another example of a greedy quantidier because it is an item that can be matched multiple times.  

### OR Operator

### Character Classes
- Referring to the characters inside the square brackets, they are the ones being matched. For instance `[abceasyas123]` will match `a`, `b`, `c`, `d`, `e`,`a`,`s`,`y`,`a`,`s`,`1`,`2`, or `3`. This states <i>any</i> character between `a` and `z` will match.

### Flags
- A flag regex would be considered `i` at the end of `\b[a-z0-9#$_-]+@[a-z0-9]+\.[a-z]{2,3}\b/i`, preventing us from having to type out `\b[a-zA-Z0-9#$_-]+@[a-zA-Z0-9]+\.[a-zA-Z]{2,3}\b/i`(note the addition of `A-Z`, with the `i` we don't need to put that in there as the flag provides that for us!). There is also the `g` flag, the `g` flag which provides a global search for the Regex definition matches, but you will have to include the upper cases.

### Grouping and Capturing
- 

### Bracket Expressions

- Brackets `[]` define the character class. Any character inside the brackets will produce a match the Regex pattern. This is unless the negate character(`^`) precedes the characters in the class.`[a-z]` defines any character class that is within the alphabet (including both upper/lower cases because of `i`).


### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
