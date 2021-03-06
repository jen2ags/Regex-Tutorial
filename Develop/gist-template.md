# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

An anchor symbol in a regex are like declarations for a specific position in the string of characters. Anchors such as the ^ and $, determine the beginning and end of the string that will be created. 

    The ^ determines where the beginning of the string starts. 
    The $ occurs at the end of the string to show where the string ends. 

The code between the anchors is what the action is attempting to match.

### Quantifiers

Quantifiers will tell the regex engine exactly how many occurances of characters, character class, or group there will be. 

The following are the different types of regex quantifiers that you can see in any regex:

{ n }, { n , }, { n , m }, *, +, ?

For example, in the email matching regex, the quantifiers used are + and { n, m }.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

The + means that these characters can occur one or more times. The {2,6} means that the characters within the bracket must generate at two characters but at most can only generate six characters.

### OR Operator

### Character Classes

Character classes tell the regex engine what type of character can be used when matching. They will appear inside the [] (square brackets).

There are many different character classes. They can include, letters, numbers, and any symbol as long as they are included inside the square brackets. 

The following are the different types of character classes that are found in our email matching regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

[a-z] Means that any lowercase letter from a-z can be used.
[0-9] Means that any number between 0-9 can be used.
[_\.-] Means that any of these symbols may be used. The \. means that this is an excaped character and just means a regular "."
[\d] Means that any digit may be used.

### Flags

### Grouping and Capturing

Capturing groups use () to group together character classes and quantifiers so they will apply to the matching inside the parenthesis. As you can see, in the email matching regex, we have 3 different groups:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

([a-z0-9_\.-]+) Capturing Group #1

([\da-z\.-]+) Capturing Group #2

([a-z\.]{2,6}) Capturing Group #3


### Bracket Expressions

Brackets tell the regex engine what it should be looking for to match. The bracket expression contains your character classes. For exampl, from our email matching regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

[a-z0-9_\.-] This bracket expression tells the regex engine that it can look for any letter a-z, any number 0-9, underscore (_), dot (\.), and dash (-).

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
