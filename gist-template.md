# RegEX

Welcome to my tutorial describing and helping with getting a better understanding of what RegEx is. By definition RegEx stands for Regular expressions and they are special strings representing a pattern to be matched in a search operation. Now how do we do this by searching for specific patterns with special characters known as unicodes.

## Summary

I will be breaking down the responsibilities of indiviual components of this regular expression: /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/ This expression certifies that a user inputs a valid email address.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
The two Anchors in regex are "^" and "$".
"^" means that the following code must appear at the beginning of the string.
"$" means that the preceding code must appear at the end of the string. The regular expression contains both of them.
### Quantifiers
the two Quantifiers in this regex includes the "+" and"{ }"
"+" will connect the users email name + email service + .com. 
"{}" for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].
### Character Classes
The two Character Classes are "/d" and "."
"\d" is used to match any digit characters. 
"." is used to match any characters.
### Grouping and Capturing
Grouping and Capturing is done with ( ) in regex.
/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/
Anything within a set of parentheses is taken in a single group, which allows all the information inside to be captured as a single unit.
The first group in this expression is ([a-z0-9_\.-]+) that matches the user email name. The second capturing group is ([\da-z\.-]+) which will match the email service. Then lastly, capture group #3 is ([a-z\.]{2,6}) to capture the .com.
### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

My name is Joseph Hudak thanks for taking the time to read this and here is a link to my github https://github.com/Magicalburritos
where you can check out more stuff i am working on.
